This repository https://github.com/OBF/wiki is a GitHub pages site rendered at
https://obf.github.io/wiki/ using Jekyll.

The content is CC-BY 4.0 licensed, having been exported from the OBF MediaWiki
installation which was self-hosted at https://www.open-bio.org/wiki/ and used
from December 2005 until May 2019 when the only edits were to guide visitors
to the replacement WordPress site at https://www.open-bio.org/ instead.

Conversion History
==================

The conversion was run in February 2024 as folloows, with the final MediaWiki
revision from July 2020.


MediaWiki export
----------------

On the MediaWiki server we ran the following, reporting 5314 revisions including
files like images:

```
$ php ~/www/w/maintenance/dumpBackup.php --conf ~/www/w/LocalSettings.php \
  --full --include-files --uploads > obf_mediawiki_dump_2024-02-05.xml
$ bzip2 obf_mediawiki_dump_2024-02-05.xml.bz2
```

We then copied the compressed XML dump to a Linux computer with git and pandoc.

Record MediaWiki history in git
-------------------------------

The [mediawiki_to_git_md](https://github.com/peterjc/mediawiki_to_git_md)
version 2.0.0 script ``mediawiki_to_md.py`` was used to turn the MediaWiki
revisions into a chronological git history, recording each page as a MediaWiki
file (with an extra header containing the page title), and any uploaded files
like images:

```
$ ./xml_to_git.py -i ./obf_mediawiki_dump_2024-02-05.xml.bz2 -p ""
```

These commits we all dated as per the MediaWiki history, along with our best
effort to map the usernames to their name and email as used on GitHub.

During the import multiple usernames were flagged as spam and the commit
comments labelled as unwanted. This along with searching the history for
reverts allowed the git history to be cleaned up with the interactive git
rebase command (``git rebase -i XXXXX --empty=drop``). Only a few cases
required manual conflict resolution as most spam was reverted via the
MediaWiki interface.

Convert MediaWiki files to Markdown for GitHub Pages
----------------------------------------------------

The [mediawiki_to_git_md](https://github.com/peterjc/mediawiki_to_git_md)
version 2.0.0 script ``./mediawiki_to_md.py`` was used to turn the final
MediaWiki files (with custom headers recording their titles) into Markdown
using [pandoc](https://pandoc.org/).

```
./mediawiki_to_md.py -i . -p ""
```

This script also handled internal redirects between pages. For example
``BioPython.mediawiki`` was a redirect to ``Biopython``, while file
``Biopython.mediawiki`` became ``Biopython.md`` and included the
redirect-from entry in the header:

```
redirect_from:
 - wiki/BioPython
```

This required the following in the Jekyll ``_config.yml`` file:

```
plugins:
- jekyll-redirect-from
```

Final edits by hand
-------------------

External redirects done with the inter-wiki addon
[issue #1](https://github.com/OBF/wiki/issues/1) were resolved
manually, in many cases the old BioPerl wiki page no longer existed.

There were snippets of HTML left over from the migration
[issue #2](https://github.com/OBF/wiki/issues/2), for example the blue
box on the main page. These were addressed by hand. 

The GitHub Pages theme and styling was also done separately.
