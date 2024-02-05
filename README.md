This repository https://github.com/OBF/wiki is a GitHub pages site rendered at
https://obf.github.io/wiki/

The content is CC-BY 4.0 licensed, having been exported from the OBF MediaWiki
installation which was self-hosted at https://www.open-bio.org/wiki/ and used
from December 2005 until May 2019 when the only edits were to guide visitors
to the replacement WordPress site at https://www.open-bio.org/ instead.

The conversion was done by running the [MediaWiki dumpBackup.php
script](https://www.mediawiki.org/wiki/Manual:dumpBackup.php), and then
[mediawiki_to_git_md](https://github.com/peterjc/mediawiki_to_git_md) which
version 1.2.2 uses [pandoc](https://pandoc.org/) to convert each revision of
the MediaWiki export into Markdown pages in a git repository. This required a
manually compiled mapping of old MediaWiki usernames to names and emails as
used on GitHub, which could be done for the majority of contributors.

Specifically on the MediaWiki server we ran the following, reporting 5314
revisions including files like images:

```
$ php ~/www/w/maintenance/dumpBackup.php --conf ~/www/w/LocalSettings.php \
  --full --include-files > obf_mediawiki_dump_2024-02-05.xml
$ bzip2 obf_mediawiki_dump_2024-02-05.xml.bz2
```

We then copied the compressed XML dump to a Linux computer with git and pandoc.

Note that spam edits, talk pages, and user pages were not converted.
The conversion was run in February 2024, with the final MediaWiki revision
from July 2020.

The content here is considered archived, with only changes to fix the display
or potentially updating of URLs planned from here onwards.
