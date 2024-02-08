---
title: Codefest 2010
permalink: Codefest_2010
layout: wiki
---

OpenBio Codefest 2010 will take place July 7th and 8th, 2010 in
conjunction with [BOSC 2010](BOSC_2010 "wikilink"). This is an
opportunity for OpenBio developers from projects like
[BioPerl](http://bioperl.org), [BioJava](http://www.biojava.org),
[Biopython](http://biopython.org), [BioRuby](http://www.bioruby.org),
and [EMBOSS](http://www.emboss.org) to work collaboratively on improving
Open Source Bioinformatics code.

## Goals

OpenBio projects are typically coordinated remotely, with users from all
over the world contributing and organizing themselves through mailing
lists and IRC chats. Additionally, contributors work on these projects
in their spare time, coordinating improving the projects with their day
jobs and life outside of the computer. The objective of the Codefest is
to give these talented developers a chance to be fully focused on the
projects for a few days, interacting in real time. Previous
[Hackathons](Hackathons "wikilink") have been immensely successful at
producing new high quality code and innovative project developments.

The general aim of the Codefest is improving the accessibility,
functionality and interoperability of the existing libraries. The
specific goals are determined based on the interests of attending
members and inputs of sponsors. Some current areas of topic discussion
are:

### Cloud computing

Improving the presence of OpenBio libraries on distributed computing
environments like [Amazon Elastic Compute
Cloud](http://aws.amazon.com/ec2/) and
[Eucalyptus](http://open.eucalyptus.com/). Ntino has written up an
excellent project proposal available for [download in pdf
format](BOSC_2010_Cloud_BioLinux.pdf).

Initial work has started to develop an automated build environment that
incorporates the [Cloud
BioLinux](http://www.jcvi.org/cms/research/projects/jcvi-cloud-biolinux/overview/)
and [bioperl-max](http://fortinbras.us/bioperl-max/) efforts. See the
[blog
post](http://bcbio.wordpress.com/2010/05/08/automated-build-environment-for-bioinformatics-cloud-images/)
for full details. Code and configuration files are available from a
[GitHub
repository](http://github.com/chapmanb/bcbb/tree/master/ec2/biolinux/).
The post outlines several areas of improvements which could be targets
for focused work at the Codefest.

### Semantic Web

[The 3rd DBCLS BioHackathon](http://hackathon3.dbcls.jp/) focused on the
Semantic Web technologies in bioinformatics. As a result, in addition to
the [UniProt](http://uniprot.org/), several database providers including
[DDBJ](http://www.ddbj.nig.ac.jp/), [PDBj](http://www.pdbj.org/) and
[KEGG](http://www.kegg.jp/en/) have started to generate their data in
RDF. These Linked Data can be queried by SPARQL and initial attempts to
provide high level library for biological queries were made by
[BioPython](http://biopython.org/) and [BioRuby](http://bioruby.org/)
groups. We propose to continue this challenge with all OpenBio projects
to make a standard interface (query builder, ontology mapping etc.) for
major biological SPARQL endpoints and handling RDF files.

To achieve this goal, we also need to develop an integrated/distributed
triple store such as
[BioGateway](http://www.semantic-systems-biology.org/). From our
experience, to generate and store a large scale RDF triples is still a
major issue even with standard triple stores. Additionally, we will try
to convert biological queries in natural language to SPARQL with a NLP
technology.

## Location

- July 7, 2010 (10am to whenever) -- Countway Library of Medicine at the
  Harvard Medical School, 10 Shattuck St Boston
  [1](http://maps.google.com/maps?oe=utf-8&rls=org.mozilla:en-US:official&client=firefox-a&um=1&ie=UTF-8&q=countway+library&fb=1&gl=us&hq=countway+library&hnear=Boston,+MA&cid=0,0,5764501267301494561&ei=DKgjTMqrGoT6lwf00aS4AQ&sa=X&oi=local_result&ct=image&resnum=1&ved=0CBMQnwIwAA)
  - Getting there: take the E-line green line train (direction Heath St)
    to the Brigham Circle stop. Cross over to the right side of the
    street and walk back a bit in the direction from which you came.
    There is a passageway directly before the Harvard School of Public
    Health; walk down the steps into the courtyard area behind the
    Harvard School of Public Health, and continue straight back through
    the courtyard and up the steps on the other side. Turn left at the
    top of the stairs and you will see the Countway Library on your
    left. When you arrive, the security guard should have your name, but
    if not, tell him you are attending the Hackathon and he will let you
    through. If you get lost use the [PDF
    map](Brigham_Circle_-_Countway_Map.pdf)
    as a guide.

<!-- -->

- July 8, 2010 (10:30am to whenever) -- Massachusetts General Hospital
  (MGH), Simches Research Building, Room 3130 [185 Cambridge Street,
  Boston,
  MA](http://maps.google.com/maps?hl=en&source=hp&q=185+Cambridge+St,+Boston,+Suffolk,+Massachusetts+02114&um=1&ie=UTF-8&hq=&hnear=185+Cambridge+St,+Boston,+MA+02114&gl=us&ei=qeteS_eUGoy1tgeDyKjwCw&sa=X&oi=geocode_result&ct=image&resnum=1&ved=0CAsQ8gEwAA)
  - Getting there: The three closest [MBTA](http://www.mbta.com/) stops
    are 'Charles/MGH' (Red Line), 'Bowdoin' (Blue line) and 'Government
    Center' (Green line). All three are located next to Cambridge
    Street. From the Red Line stop, walk away from the river; walk
    towards the river from either the Blue or Green line. Simches is
    located slightly off Cambridge Street -- the closest landmark on
    Cambridge Street is a big yellow Au Bon Pain. Walk up the stairs
    next to the Au Bon Pain and you'll be in a parking lot: the Simches
    building is located straight in front of you across the parking lot,
    to the left of the Whole Foods and CVS. Walk in the lobby and the
    security desk should have a badge for you. You can take the
    elevators up to the 3rd floor. Room 3130 is down the only
    non-secured corridor and is on the left side just past the
    cafeteria.

## Resources

- [Amazon Web Services](http://aws.amazon.com/) -- We will be able to
  use EC2 and other Amazon services thanks to [Amazon
  grant](http://aws.amazon.com/education/) support for a proposal put
  together by Steffan Moellar. Many thanks to Amazon for supporting the
  initiative and Steffan for putting together the application.
- [Eucalyptus](http://www.eucalyptus.com/) -- The [Universitätsklinikum
  Schleswig-Holstein](http://www.uk-sh.de/index.phtml?NavID=676.467.4&La=4&switch_la=1&back_qs=NavID%3D676.467.4)
  is sponsoring a 12 node local Eucalyptus cloud for testing and
  development. Thanks again to Steffan for making this available.

## Sponsorship

Space and internet for the Codefest are kindly provided by the [Harvard
School of Public Health Bioinformatics
Core](http://www.hsph.harvard.edu/research/bioinfocore/) and
[Massachusetts General Hospital](http://www.mgh.harvard.edu/). We are
actively seeking sponsors to help supplement the travel, lodging and
meal costs for developers. If you're interested in contributing to Open
Source development in Bioinformatics and helping to direct the focus on
the Codefest, please contact Brad.

## ToDo List

Add your goals and plans for the Codefest here. This is a brainstorming
section to help us organize ourselves.

### Cloud computing

Work for the current [community bioinformatics
image](http://bcbio.wordpress.com/2010/05/08/automated-build-environment-for-bioinformatics-cloud-images/)
([framework on
GitHub](http://github.com/chapmanb/bcbb/tree/master/ec2/biolinux/)):

- Perl library support and useful package list
- Java library organization and expand useful packages
- Provide packaging for missing programs. See comments at the end of the
  [Package
  config](http://github.com/chapmanb/bcbb/blob/master/ec2/biolinux/config/packages.yaml)
  for some targets.
- Documentation: especially targeted at new users.
- Produce an automated manifest for an AMI, listing versions of all
  installed packages and libraries.
- Provide standard data like indexed next-gen genomes, blast databases,
  and so on via EBS snapshots.
- Automation to build AMI and roll out to Amazon on a bi-weekly/monthly
  basis based on latest code.
- Website with documentation, AMI history.
- Testing on [Eucalyptus clouds](http://ecc.eucalyptus.com/).
- Titus Brown's post on [using cloud computing to teach a next-gen
  sequencing
  course](http://ivory.idyll.org/blog/jun-10/ngs-course-postmortem.html).
- Richard Holland's post on [getting started with Amazon
  EC2](http://blog.eaglegenomics.com/?p=17).

### Suggested Additions for Cloud computing image

#### Perl

#### Ruby

#### Python

#### Java

#### Data

- [UniRef](ftp://ftp.ebi.ac.uk//pub/databases/uniprot/current_release/uniref)
  - UniRef50 and UniRef90, and if you've got the space, UniRef100, too.

### Semantic Web

- Building SPARQL endpoints of DDBJ RDF, PDBj RDF, MEDLINE, KEGG and
  UniProt.
- Complete supports for SPARQL endpoints in BioRuby and BioPython. If
  possible, BioPerl and BioJava as well.
  - [Brief introduction to RDF/SPARQL in
    OpenBio](http://hackathon3.dbcls.jp/wiki/ImplementationBootcamp)
  - [Example queries against
    Bio2RDF](http://sourceforge.net/apps/mediawiki/bio2rdf/index.php?title=Demo_queries)
  - [Example queries against
    BioGateway](http://www.semantic-systems-biology.org/biogateway/querying)
  - [SemWeb:PDB2RDF](SemWeb:PDB2RDF "wikilink")
  - [SemWeb:Bio2RDF_Endpoints](SemWeb:Bio2RDF_Endpoints "wikilink")

### Bioperl/BioSQL

- Include SQLite support in BioSQL
- DBIx::Class integration with BioSQL
- A bit on Moose and Perl 6

### Key signing

- Sign Open PGP keys for OBF project release managers, see e.g. [The
  Keysigning Party
  HOWTO](http://cryptnet.net/fdp/crypto/keysigning_party/en/keysigning_party.html)

## Attendees

- [Brad Chapman](http://bcbio.wordpress.com/)
- [Oliver Hofmann](http://www.hsph.harvard.edu/research/oliver-hofmann/)
- [Mark A. Jensen](http://www.bioperl.org/wiki/User:Majensen)
- [Hilmar Lapp](http://www.bioperl.org/wiki/User:Lapp)
- [Michael Heuer](http://www.biojava.org/wiki/Michael_Heuer)
- [Chris Fields](http://www.bioperl.org/wiki/User:Cjfields) - Arriving
  Wed around 2pm
- [Ntino Krampis](http://www.linkedin.com/in/agbiotec)
- [Tim Booth](http://nebc.nox.ac.uk/nebc/about-us/people)
- <s>[Peter Cock](http://www.scri.ac.uk/staff/petercock)</s> (Unable to
  attend)
- [ Kam Dahlquist](User%3AKdahlquist "wikilink")
- [John David N. Dionisio](http://myweb.lmu.edu/dondi)
- Steffen Moeller
- [Richard Holland](http://www.biojava.org/wiki/User:Rholland) (TBC)
- [Bela Tiwari](http://nebc.nox.ac.uk/nebc/about-us/people)
- <s>[Oliver Buckley](http://nebc.nox.ac.uk/nebc/about-us/people)</s>
  (Changed job)
- [ Dominique Belhachemi](User%3ADomibel "wikilink")
- [Toshiaki Katayama](http://www.linkedin.com/in/toshiakikatayama)
- [Mitsuteru NAKAO](http://www.linkedin.com/in/nakaomitsuteru)
- [Dave Messina](http://www.bioperl.org/wiki/User:Dave_Messina)
- [Christian Zmasek](http://www.linkedin.com/in/cmzmasek)
- Kimberly Begley
- [Akira KINJO (PDBj)](http://jp.linkedin.com/in/akirakinjo)
- [Naohisa Goto](http://www.linkedin.com/in/ngoto)
- [Yasunori Yamamoto](http://purl.org/yayamamo/home)
- [Raoul J.P. Bonnal](http://it.linkedin.com/in/raoulbonnal)
- [Atsuko Yamaguchi](http://www.linkedin.com/in/atsukoyamaguchi)
- Christopher Bottoms (+ wife Marcie, and dau. Zebadee)
- [James Taylor](http://bx.mathcs.emory.edu)
- [Enis Afgan](http://bx.mathcs.emory.edu)
- [Dannon Baker](http://bx.mathcs.emory.edu)
- [Shuichi Kawashima](http://jp.linkedin.com/in/shuichikawashima)
- Jin-Dong Kim
- [Heikki
  Lehvaslaiho](http://sa.linkedin.com/pub/heikki-lehvaslaiho/1/974/377)
- [Eric Talevich](http://etalog.blogspot.com/)
- [Marc-Alexandre Nolin (Bio2RDF)](http://bio2rdf.org/)
- [Scott Cain](http://scottcain.net/)
- [Aaron
  McKenna](http://www.broadinstitute.org/gsa/wiki/index.php/Main_Page)
- [Roger A Hall](http://search.cpan.org/~rogerhall/)

Feel free to add yourself if you are interested. We are happy to have
you.

## BBQ

After two days of hard work, there will be a celebratory BBQ at [Brad's
house in
Somerville](http://maps.google.com/maps?hl=en&q=35+Partridge+Avenue+Somerville,+MA+02145&um=1&ie=UTF-8&hq=&hnear=35+Partridge+Ave,+Somerville,+MA+02145&gl=us&ei=3ckYTKzOL4OC8gbd_qDODA&sa=X&oi=geocode_result&ct=image&resnum=1&ved=0CBQQ8gEwAA)
the evening of July 8th. All are welcome for drinks and whatever magic I
can whip up on my little charcoal grill.

The easiest way to get there is via cab. From Mass General Hospital,
walk up Cambridge Street a few blocks to the Liberty Hotel where there
is a cab stand. Ask the cab driver to take you to Medford Street in
Somerville, via McGrath Highway. Partridge Avenue is located off Medford
Street, on the right a few blocks after Central Street. I'll pass out my
cell phone number to everyone during the coding sessions if more
directions are needed on route.

## Discussion

We welcome any thoughts from interested participants. Please direct
discussion to the OpenBio mailing list: <open-bio-l@lists.open-bio.org>.

For short-lived coordination tasks during the hackaton, an IRC channel
has been setup on FreeNode: \#codefest

Please use the hash tag \#bosc2010 on twitter to help remote folks
follow the discussion.
