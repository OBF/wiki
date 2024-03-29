---
title: BOSC/Prepare for Vienna
permalink: BOSC/Prepare_for_Vienna
layout: wiki
---

This page has been set up to provide a forum for discussion regarding
the planning of BOSC 2007.

BOSC Mandate:

1.  provide developers with a forum for displaying the results of their
    development efforts to the wider research community;
2.  provide a focused environment for developers and users to interact
    and share ideas about software development, and practical techniques
    in bioinformatics;
3.  Inform the Research Community of important developments occuring
    within the Open Source Bioinformatics Developer community.

To this end, the BOSC conference must endeavor to meet these goals using
the 16 hours of time that we are alloted during the two day ISMB SIG.

Comments/questions to consider:

1.  How do we facilitate the integration of disperate communities, or at
    least avoid excessive fragmentation. Suppose we create separate
    sessions for, say, Project Updates, and Emerging Informatics. What
    is going to prevent the developers from choosing to skip the
    Emerging Informatics session because they dont get anything out of
    it? Isn't one goal of BOSC to provide a forum for the discussion of
    new areas where Bioinformatics Infrastructure, especially Open
    Source Infrastructure, is needed? Remember that it is perfectly
    acceptable for people to wander from SIG to SIG with the price of
    their admission. They are not a captive audience.
2.  In relation to the above, how do we prevent one community from
    completely taking over the conference for their own purposes?
3.  How do we ensure that BOSC stays relevant to the wider ISMB-SIG
    audience? Is this important?

## requirements and deadlines

- Friday Dec. 15th. Submit Proposal for BOSC to ISCB Organizing
  Committee
- [Proposal Requirements](http://www.iscb.org/ismbeccb2007/sigs/)
- ??? Some time in Dec. call for community feedback if we want input for
  categories/speakers to create/invite
- ??? Early January. Announce and Call for Papers??? BOSC 2007
- ??? Secondary Call???
- ??? Submission due date
- ??? A few days before June 1(early reg deadline) Announce Accepted
  Speakers
- July 19,20 BOSC 2007

## ideas

1.  Create separate sessions for different categories of talks. These
    should include, but not be limited to, a section for project updates
    by the developers of various projects. Define better requirements
    for acceptance of submission to each of the talk sessions, and
    communicate these requirements in the call for speakers.
2.  Shorten the talk times, to allow more time for discussion and
    questions.
3.  Expand on the idea of the keynote speaker. Create a special session
    for invited speakers. Call for greater involvement from the Open
    Source Developer community to decide which areas to concentrate on,
    and which experts to invite.
4.  Organize a forum for informal, relaxed discussion and socializing
    among BOSC attendees, such as a dinner or visit to a local pub after
    the days activities.
5.  Organize a forum for inter-SIG collaboration. Possibly create a slot
    to allow someone from the other SIGs to present needs, ideas to the
    Open Source Community, while also supporting the export of our own
    ideas to their SIGs.
6.  Create A Developer Challenge Forum. The year before BOSC (possibly
    at the end of each BOSC), teams of developers would be called on to
    submit a proposal for the development of a significant software
    product. Each team would be given a wiki on the upcoming BOSC 2XXX
    wiki site where they would communicate significant problems,
    resolutions, and achievements. At BOSC, there could be a session
    where these teams present the results of their work. If we had
    outside funding, we might be able to award travel fellowships to the
    team voted to have done the best work by the BOSC community, but we
    might need other criteria to be met before they could be entered
    into the competition?
7.  Do more targeted invitations to people who would give interesting
    talks. Hilmar pointed out the zebrafish project does usability
    testing including videotaping people using their system. I would be
    interested in knowing more about that.

## Thoughts from Andrew

This is something I wrote up for the board list on a thread related to
this topic. I've extracted the part where I talk about what I want to
see in a conference.

### I want something very hands on.

"hacker sessions" in old-skool parlance. The current phrase is "bar
camp". See <http://en.wikipedia.org/wiki/BarCamp> and
<http://barcamp.org/> .

People don't just show up and give talks or demos. They also come to
code. For examples mostly based on this year's abstracts, people might
write new services for BioMOBY and Taverna, try out ZMap and provide
feedback, use some of the BioPostgres extensions, or learn a bit of Ruby
through bioruby. BOSC is open source so we have the advantage that
anyone can install the software on their laptops.

This means some preparation beforehand, like the "Ridiculously Easy MOBY
Service Creation" document at
<http://biomoby.open-bio.org/CVS_CONTENT/moby-live/Java/docs/deployingServices.html>

I don't like training seminars though.

A popular event I've seen elsewhere is a "bake off" as a way to
compare/contrast two technologies. To me the most famous of these was
"the Great CHI'97 Browse-Off" was reproduced in part at BayCHI in
<http://www.baychi.org/calendar/19970812/>

One topic: "using your web framework of choice, make a blah" where blah
can be "biosql browser" or "BLAST job manager" or ...

Another: load the same data set into different tools (eg, annotation
data in Apollo, GBrowse, etc) and evaluate some common use cases, a la
the browse off.

### I want discussion about newer technology

Some of the hot topics over the last couple of years: P2P, tagging and
folksonomies, AJAX, Ruby on Rails, Web 2.0. How might these affect
bioinformatics? Collaborative tagging of GenBank records? What about
using off-the-shelf P2P libraries for collaborative curation? Dojo-style
widget sets for highly-interactive browser-based sequence display?
Setting up RSS/Atom feeds for job process notification?

The current BOSC schedule is derived from a scientific program where
people show results. By its nature it won't include wild ideas which may
be the seeds of the next generation of software.

### I want more emphasis on software development

I mean this as something stronger than "programming" but not to the
point of "software engineering" (I don't think the field is mature
enough yet for there to be "engineering.")

I think bioinformatics - and chemical informatics and structural biology
and molecular modeling - are years behind the times in how to write
software. Here are some things to think about:

- how many bioinformatics GUIs support undo/redo? How does one implement
  such a system?

<!-- -->

- how many applications had any usability/human-centered design/user
  testing as an explicit part of the development process?

<!-- -->

- do any of the projects have a buildbot system continuously checking
  that the code in version control works, along with enough tests to
  make that check meaningful?

<!-- -->

- what do the web-based projects used for automated testing of their
  servers?

<!-- -->

- does anyone do fuzz testing? Security analysis? What about a "break my
  web app" session where us black-hat wannabes find flaws and exploits
  in others' servers?

That's not saying commercial non-bioinformatics software do these. I'm
saying that bioinformatics software, and the culture of writing
bioinformatics software, should stretch and include good modern
development practices and techniques.

But this has nothing to do with science and nearly every software
developer in this field has a science background so regards these topics
as having less importance or uninteresting, assuming any knowledge at
all. So says my experience.

That lack of interest, btw, is part of a general frustration I have with
scientific software development. Good software is often seen as second
to good science, when it should be an essential part of doing good
science. I've found many of the talks at BOSC pretty boring because they
only cover programming. I'm very good at programming and don't need a 20
minute lecture for each topic.

Tangentially, what about a round-table discussion somewhere for people
to hear different viewpoints on a set of topics?

### closing

If a future BOSC was arranged along the above lines then I would be very
excited to go. I know of almost nothing like it in the bio/chem software
fields. The closest would be sprints and hackathons, but this isn't
either. It's more like an informally structured educational environment
in which to learn about about the state-of-the-art for software in and
outside of bioinformatics.

Doing this would almost totally alter the current BOSC format. Such a
change may be too much for next year, but perhaps chaning one day would
work. The first day is my preference.

Would people go for it? I don't know. I would like to think so.

## Darin Comments

### Initial Thoughts

I think that Andrew's thoughts point out the divergence in 'needs'
between the typical BOSC attendee (currently a subset of the typical
ISMB attendee), and the typical OBF programmer. I, too, would like to
see many more of his ideas in BOSC. However, finding the right balance
between the Traditional (presentation-of-results/project updates) and
the Unconference which will maitain a base of ISMB subset attendees,
while drawing back in the OBF developers will be tricky. It is pretty
clear that BOSC doesnt survive serving only one of these two
populations.

Unconferences require more infrastructure than what ISMB currently
provides (A/V + screens). We havent even been granted free WIFI yet in
the conference rooms (I have asked for this repeatedly). This year it
was there in principal, but the signal was too weak to use. We would
need to set up our own wifi on the wire that they provide us. Not a huge
obstacle, but something to think about.

### Bar Camps

I really like the idea of the Bar Camp. We could devote all, or part of
the second day to this, and keep the first day a little more traditional
( I know Andrew wanted the first day to be changed). We could then allow
presenters to generate enthusiasm during their presentations for a
barcamp sessions the next day. We have seen this in its infancy in many
occasions where people did the main talk, and a demo during the
lightning talk sessions.

### Bake Offs

This might be easier to generate by inviting key developers of competing
projects (EnsEMBL vs USCD, bioPerl vs bioPython, etc) to demonstrate a
sophisticated problem that their system solves that the other system
does not, or some other way of playing key stakeholders off against each
other for our mutual enjoyment/education. We could call for nominations
from the OBF developer community to decide who to invite.

### New Technologies

Currently, any conference is going to be generated by the miliue of its
community. The OBF developer community currently doesnt have any
examples of these technologies (although I, myself, have thought about
how to use a del.icio.us framework for annotation). You could create a
session where people are invited to talk about potential uses of one or
more of these technologies. However, these often lead to the same
criticism that is generated by those trying to get the OBF developer
community to set its sights on new areas where informatics
infrastructure is weak or nonexistant. Basically, you get the 'what did
that talk do for me' mentality from both communities.

### Software Engineering Best Practices

This could be a separate session. It would probably be best to invite
the OBF developer community to nominate, and vote on one or two projects
to be invited to talk about their software development practices. The
'Break My XXX' would probably be best as a BarCamp session.

## Links of Interest

[ Example Schedule](Prepare_for_Vienna/ExampleSchedule "wikilink")

[ISMB 2007 Deadlines](http://www.iscb.org/ismbeccb2007/deadlines)

## Schedule Ideas

1st Day:  
8:35 Call To Order, Announcements while people mill in  
9:00 Keynote: Carole Goble On Significant Challenges to Developing
Bioinformtics Software  
10:00 Currently Intractable Problems In Bioiformatics: Five to ten
minute talks presenting a hard area of computer science or
bioinformatics relevant to the community and as yet not thoroughly
solved. Talks would be of the form of a use case which currently cannot
be satisfied with readily available toolkits and a summary of the
problem.  
10:30 coffee  
10:50 More Currently Intractable Problems  
11:50 Break For Lunch  
1:15 Talks on developments or ideas for using New Informatics
Technologies to support Biological Research (10 minute talks on
folksonomies, web 2.0, Rest, SOAP, etc.)  
2:45 Project Update Section: Lead Bio\* Developers or their Designates
are invited to present updates of major developments on their projects  
3:30 coffee  
3:50 OBF CD Session: Session laying the groundwork for the creation and
management of an single CD of OBF applications, libraries for easy
installation. The goal is to create a CD to distribute for the next
BOSC. Something like software for starving students,
www.softwarefor.org.  
4:10 Wifi Workshops: We make the wifi available (if it isnt already,
e.g. one of us needs to bring a wifi router, I'll bring mine if I have
to), and open it up to people to present interactive demos, network with
users, etc in small, BOF-like subgroups within the hall. This would be a
wifi enhanced BOF for people to use to demo their system, or interact
with users.  
5:30 Dismiss for Dinner (to be announced)  
  
  
2nd Day:  
8:35 Call To Order, Announcements while people mill in  
8:45 Keynote: Insert important Bioinformatics Person Here...????  
9:30 Typical BOSC Talks, e.g. abstract submission, review, and
acceptance before the conference  
10:30 coffee  
10:50 More Typical Talks  
12:00 Lunch  
1:15 Intro Software Design session: Get someone to talk about Software
Design (Maybe Andrew could give the talk he always wanted to hear :) )  
1:40 Invite people to present on Design Practices in their Open Source
Project, or an Open Source Project they have used and were happy with
(we dont want gripe sessions, do we)?  
3:30 coffee  
4:00 Ideas for Solving Currently Intractable Problems in Bioinformatics:
Here is the chance for developers to present ideas for using current
technologies, or developing new technologies, to solve issues presented
in the Keynote Session on Day 1. Those presenting problems in the first
day are required to summarize ideas revolving around their submitted
problem  
5:30 Dismiss

## BOSC 2007

<img src="Pear.png" title="The Bosc Pair" />

The 8th annual Bioinformatics Open Source Conference
([BOSC](../BOSC "wikilink") 2007) will take place in [Vienna,
Austria](wp:Vienna,_Austria "wikilink"), as one of several Special
Interest Group (SIG) meetings occurring in conjunction with the [15th
International Conference on Intelligent Systems for Molecular
Biology](http://www.iscb.org/ismbeccb2007/).

This year is shaping up to be very exciting. We have changed our format
to add room for more development oriented talks and discussions, in an
effort to fully utilize the conference to stimulate new development
efforts in all areas of Open Source Bioinformatics Software development.
The primary focus of the conference revolves around the delineation of
areas of IT or Bioinformatics which are not well serviced by existing
toolkits. The Keynote session will be headed up by Carol Goble, of
Manchester University. Speakers in this session will be invited to
present detailed descriptions of an 'Intractible Problem In
Bioinformatics'. The last session of the conference has been setup for
speakers to present ideas for solving any of the problems presented in
the keynote session. Other sessions will be set up to allow
presentations on new Software Design Patterns, Software Engineering
ideas, and more traditional BOSC talks (see below for details and
deadlines). There will be a session of talks by developers in the major
Bio\* projects giving overviews of recent developments in their
projects. Finally, the Birds of a Feather sessions will be enhanced with
wifi to create 'Wifi Workshops'. All in all, this should be a great
conference.

## Important Dates

June 1 **Early Registration Discount Cutoff Date**  
July 19,20 **BOSC 2007**

[BOSC Eventful Group](http://eventful.com/groups/G0-001-000014747-0) :
This site provides an ICAL feed which will include all deadlines
associated with BOSC 2007  
[BOSC Announcement Blog](http://www.open-bio.org/boscblog/) : This Blog
will contain all Important BOSC announcements. You can include it in any
RSS Reader.

## Keynote Speakers

[Carol Goble](http://www.cs.man.ac.uk/~carole/)

## Fees

SIG Rate (registering for ISMB as well):  
Corporate : TBA  
Academic : TBA  
Student : TBA  
==================================================

Sig-only Rate (not registering for ISMB):  
Corporate : TBA  
Academic : TBA  
Student : TBA  

## Agenda

### Notes on Submissions

`The Open Bioinformatics Foundation is dedicated to promoting the practice and philosophy of Open Source Software development within the `  
`Biological Research Community. To promote this mission, the organizing committee will favor submissions for projects that apply a recognized `  
`Open Source License, or adhere to the general Open Source Philosophy.`

See the following websites for further details:

- [Recognized Open Source Licenses](http://www.opensource.org/licenses/)
- [Definition of the Open Source
  Philosophy](http://www.opensource.org/docs/definition.php)

All submissions should be emailed to the BOSC mailing list at
**bosc@open-bio.org**.

### Call for Speakers and Abstracts

This year BOSC is requesting submissions for a variety of different
venues. All submissions should be recieved by Monday, May 14th to be
considered for inclusion:

1.  Currently Intractable Problems In Bioinformatics: This session will
    follow the Keynote, and will be devoted to the delineation of areas
    of Bioinformatics or Information Technology which are currently not
    solved or serviced by the current suite of Bioinformatics Software
    in existence. Speakers are invited to submit a detailed use case
    which currently cannot be satisfied with readily available toolkits
    and a summary of the problem sufficient to engage developers into
    discussions on how to solve the problem. The last venue of day two
    will be devoted to allow attendees to present ideas for solving
    these problems. Talks for both venues will be 5 minutes long, with a
    few minutes for questions from the audience. All problems, and ideas
    for solution will be published on the BOSC web site.
2.  New Informatics Technologies in Bioinformatics: This venue is
    devoted to the development of systems which make use of newer
    Information Technology practices, such as WebServices (SOAP or
    REST), Folksonomies/Tagging, RSS, Social Networking, and other
    design patterns collectively described as [web
    2.0](http://www.oreillynet.com/pub/a/oreilly/tim/news/2005/09/30/what-is-web-20.html).
    Talks will be 10 minutes long, with a few minutes for questions from
    the audience. All abstracts will be published on the BOSC website.
3.  Open Source Software Presentations: This venue will allow speakers
    to present talks on their use, development, or philosophy of open
    source software in bioinformatics to the BOSC attendees. The
    committee will select several submitted abstracts for 10-minute
    talks, with a few minutes for questions afterward. Accepted
    abstracts will be published on the BOSC web site.
4.  Discussions of Software Design and Engineering: This venue will
    allow speakers to to present Design Practices in their Open Source
    Project, or an Open Source Project they have used and were happy
    with, or present ideas on the practice of Software Design which
    would benifit the Open Source Developer Community. Talks will be 5
    minutes long, with a few minutes for questions afterward. Accepted
    abstracts will be published on the BOSC web site.

### Call For Wifi Workshops

This year, the BOSC committee will enhance the infrastructure for what
were currently labeled Birds of a Feather sessions with a wireless
router. This will allow groups to interact with software or websites
much more while they are discussing their favorite projects. The BOSC
committee will accept ideas for these up to the last day of the
conference, on a first come-first-served basis until no more space is
left in the conference room.

### Lets Create an OBF Software CD!

This year we will be devoting a small BOSC session to the task of laying
the groundwork for the creation and management of a single CD of OBF
applications, libraries for easy installation. The goal is to start the
process create a CD to distribute for the next BOSC.

### Call for Volunteers

The BOSC Organizing Committee would like to invite attendees to take a
more active role in making BOSC a successful conference by volunteering
your services. The following opportunities for assistance exist:

- Set up, Clean up: Volunteers are needed to help set up and clean up
  any aspects of the conference room that are not done by the conference
  organizers.
- Historian/Photographers: Volunteers are needed to help record aspects
  about BOSC 2007 for future reference. Possibilities include blogging
  the conference, writing up a review article for the ISCB, etc.. The
  Photographer will take digital photographs of all speakers, recording
  each speakers name with their image name for easy inclusion on the
  BOSC summary website after the conference.
