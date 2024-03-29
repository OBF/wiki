---
title: Server software
permalink: Server_software
layout: wiki
---

''This page can be dynamic so feel free to update and add your comments.
We can archive parts by moving them to the [discussion
page](Talk:Server_software "wikilink"). Please sign your comments though
with \~\~~

## SVN

I would love to see the CVS to SVN migration happen by the end of the
year for all of the OBF projects.

What would need from the project leaders is some sort of schedule. So
you'd need to set a schedule for your project and coordinate how you
want to make the migration happen and we (well George with some of the
root-l people's help) can do the CVS to SVN changeover.

I don't think you HAVE to make a release before the changeover, but you
just need to get your project coordinated so everyone knows about the
ways to get code out.

- BioPerl has a preliminary CVS to SVN [migration
  page](http://www.bioperl.org/wiki/CVS_to_SVN_Migration) on the wiki to
  track progress; it just needs to be updated and eventually moved into
  the full SVN docs once they are up.
  --[Cjfields](User%3ACjfields "wikilink") 11:59, 29 October 2007 (EDT)

### How will people access the machines?

- We will still have people use SSH to get onto the dev.open-bio.org
  machine to make commits so we will still have to give shell accounts
  on the dev machine.
  - for security reasons we have chosen not run any apache or webdav on
    dev so we can't do SVN over https. I would be willing to consider
    it, but I don't know what the potential security flaws are here and
    our code repositories are an important asset so we have tried to
    keep the machine as locked down as possible.
- We will rsync the repository from dev to
  [code.open-bio.org](http://code.open-bio.org) (or possibly using
  svnsync i.e. [svnsync
  info](http://journal.paul.querna.org/articles/2006/09/14/using-svnsync/).
- anonymous SVN checkout and Browsing can be done via
  <http://code.open-bio.org>
  - possibly consider installing trac on <http://code.open-bio.org/> as
    a testbed too?

ChrisD - what do you think? Can we go ahead and get and start the wheels
turning on testing all of these things so that once a project is ready
to transition we can just implement the changeover in a few hours? I
know you have svnweb installed - is there any more testing that needs to
be done? Can you look either rsync or svnsyncing the test bioperl
repository in /home/svn-repositories?

## Web 2.0 @ OBF

### News Server

Most projects aren't really using the news servers
([bioperl.org/news](http://bioperl.org/news)). It is worth keeping these
installed? Should we consolidate things to a single newsfeed
([news.open-bio.org](http://news.open-bio.org/)) with projects as
categories instead? I was hoping that projects would be able to
designate some people to post summaries of list traffic and project
progress through the news system, but I know this takes a lot of time.

- I think consolidating the new feeds would be fine; we can always
  categorize/tag the posts. Speaking as one who wrote them up for a
  brief time, mailing list summaries are quite time-consuming, so
  finding a way to semi-automate it might be easier (I think the Perl6
  list used to do this). --[Cjfields](User%3ACjfields "wikilink") 11:56,
  29 October 2007 (EDT)
- Consolidating them would be much better to provide a nice overview of
  all O\|B\|F projects' progress. People who require more detailed
  tracking of them are used to be subscribed to the corresponding lists.
  --[Mauricio](User%3AMauricio "wikilink") 11:09, 31 October 2007 (EDT)

### Wikis

I have started working to try and consolidate the installations so
upgrades aren't such a big deal. I am sure the big meta-wiki sites have
their way of doing this as well to make it easier, but I am not sure how
I'd like to see it setup much differently.

There are quite a few orphan wiki sites right now -
[obda.open-bio.org](http://obda.open-bio.org),
[biosql.org](http://biosql.org)- is there interest in still maintaining
them? Otherwise we can redirect them to open-bio.org wiki and just flesh
out some simple 1 page project descriptions there.

A potential crazy idea is to consolidate the content into a single wiki
and just have project namespaces i.e. BioJava:Main_Page instead of the
domain names (domain names would preferentially redirect to main page of
a project i.e. biojava.org would link to
wiki.open-bio.org/BioJava:Main_Page for example. Is this a good idea?
Bad Idea? Harder to identify project branding with this I know, but some
of the definition pages like [multiple sequence alignment
tools](bp:MSA "wikilink") is harder.

- I think keeping the wikis separate is better, though I can also see
  the benefit of consolidating some of the definition pages into one
  space, as well as moving anything which relates to more than one
  project (BioSQL, OBDA, etc). Maybe use the OBF wiki for that and link
  to those pages where needed? --[Cjfields](User%3ACjfields "wikilink")
  17:51, 28 October 2007 (EDT)

<!-- -->

- I quite like [OpenID](http://openid.net) as a single sign on system
  between multiple web sites. Would be nice to install the [OpenID
  plugin](http://www.mediawiki.org/wiki/Extension:OpenID). This could be
  used to identify the same user between our different wikis
  --[Andreas](User%3AAndreas "wikilink") 07:07, 29 October 2007 (EDT)

### Ideas

If you have any feedback about how we move forward with web and web2.0
content for OBF let me know. We don't currently do much for networking
developers and users, but we could try and emphasize things like
facebook, linked in, scilink.com, or nature network as possible ways to
try and connect everyone up a little more effectively beyond the mailing
lists.

- There is also the open source social networking site
  [Ohloh](http://www.ohloh.net/). See the
  [Biojava](http://www.ohloh.net/projects/6798?p=BioJava) and
  [BioPerl](http://www.ohloh.net/projects/6685?p=BioPerl) projects
  there. --[Andreas](User%3AAndreas "wikilink") 06:40, 29 October 2007
  (EDT)

## Mailing lists

We have had a steady set of volunteers dealing with mailing lists to
moderate spam and other things. The [Volunteers](Volunteers "wikilink")
list had coordinated some of this. I'd like to check and see if this is
still working well. Can we improve how moderation is done in any way -
are there new software tools out there to make it easier to go to one
place and see all the mail that needs to be moderated?

## Recruiting drive

Part of some future stuff we'd like to do in OBF is recruit some more
people to be part of the *leadership*. This is everything from being on
the OBF [Board](Board "wikilink") to helping administer the machines,
generate content for the websites and newsfeeds, and generally recognize
the hard work that many people are doing behind the scenes. So if you
are interested or want to help recruit people, please speak up.

I would also like to see us keep more of the history pages describing
who and what have worked on the projects on the wikis. This is important
to both give people credit for the work they did and for us to keep
track of our history on the different projects.

- you could consider installing automated tools to visualize the
  historic growth of CVS and SVN projects like
  [StatCVS](http://statcvs.sourceforge.net/) and
  [StatSVN](http://statsvn.org/) --[Andreas](User%3AAndreas "wikilink")
  06:44, 29 October 2007 (EDT)

We are making strides to get the OBF as a 503(c) organization and so it
will be important to show the progress we make if we solicit donations
from corporations.

## History

Initial edits by [jason](User%3AJason "wikilink") 14:19, 27 October 2007
(EDT)
