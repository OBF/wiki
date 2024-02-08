---
title: Newsletter:2006 Winter
permalink: Newsletter%3A2006_Winter
layout: wiki
---

## Winter 2006 Open Bioinformatics Foundation Newsletter

## Open Bioinformatics Foundation Report

### President's Report

*Jason Stajich*

### 2005 O\|B\|F Board Meeting Report

*Jason Stajich* & *Hilmar Lapp*

The 2005 Open Bioinformatics Foundation board meeting was held during
the [BOSC 2005](BOSC_2005 "wikilink") conference in Detroit, MI. Several
items of business were attended to including several personnel changes.

- Past President [Ewan Birney](Ewan_Birney "wikilink") resigned and
  elected into the Board as at-large director
- [Jason Stajich](Jason_Stajich "wikilink") was newly elected into the
  Board and elected President
- [Hilmar Lapp](Hilmar_Lapp "wikilink") was elected parliamentarian

Most importantly, the Board agreed to [bylaws](Bylaws "wikilink")
governing the [OBF Board](Board "wikilink"), [OBF
membership](Project:Membership_application "wikilink") as well as
elections. This marks a defining moment in the history of O\|B\|F, as
for the first time a defined mechanism exists through which any member
can gain governing office, and volunteer his or her leadership to help
shape the future of the OBF. The O\|B\|F is ready to redefine the scope
of its vision and agenda. We extend an invitation to every interested
person to play a role in this endeavor, as a member or as a leader and
decision maker.

A broader agenda, like to facilitate and sponsor project interactions
that are otherwise impossible, will inevitably require adequate funding
resources. Therefore, as one of its future tasks the Board will need to
creatively and aggressively seek funding opportunities.

### Financial Overview

*Chris Dagdigian*

### Website and Mailing list statistics

maybe will drop this if I don't have time
[Jason](User%3AJason "wikilink") 16:31, 26 January 2006 (EST)

### BOSC Reports

*Contributed by Darin London*

Each year, the O\|B\|F sponsors the Bioinformatics Open Source
Conference ([BOSC](BOSC "wikilink")) as a Special Interest Group in
association with the International Systems in Molecular Biology
Conference ([ISMB](ISMB "wikilink")) sponsored by the International
Society for Computational Biology ([ISCB](ISCB "wikilink")). The
conferences over the last two years have been very successful, and we
look forward to continuing to serve the Open Source Bioinformatics
Community, and the wider research community in 2006.

#### BOSC 2004

[BOSC 2004](BOSC_2004 "wikilink") was held along with [ISMB
2004](http://www.iscb.org/ismbeccb2004) in [Glasgow,
Scotland](wp:Glasgow,_Scotland "wikilink"). The conference was a great
success, with 136 people in attendance. Our Keynote address featured
Wolfgang Huber, delivering an inciteful overview of the very popular
[BioConductor](http://bioconductor.org/) Open Source application system,
for which he is responsible. His talk was followed, over the course of
two days, by eleven excellent 20-minute presentations selected from a
very competitive pool of applicants; a special session on Annotation
Database Systems where the leaders in the field discussed their
representative projects; and 29 lightning talks. These talks informed us
of a huge range of Open Source/Open Standards bioinformatics software
development and usage activities within the community, including
endeavors devoted to semantically identifying life science objects,
easing the process of computationally processing the ever-growing array
of biological datasets, integrating disparate datasets, and validating
the diverse Open Source software systems available to the research
community. As always, attendees were given the opportunity to organize
Birds of a Feather discussions devoted to a diverse array of more
specialized interests after the main session each day.

#### BOSC 2005

[BOSC 2005](BOSC_2005 "wikilink") was held in conjunction with [ISMB
2005](http://www.iscb.org/ismb2005) in [Detroit,
Michigan](wp:Detroit,_Michigan "wikilink"). The meeting was very
successful, with 99 people in attendance. The meeting featured two
Keynote speakers. The first was delivered by [Jason
Stajich](Jason_Stajich "wikilink"), one of the core developers of
[BioPerl](http://bio.perl.org/). He spoke of the challenges and rewards
he has experienced in developing Open Source Bioinformatics Software,
and discussed the challenges he sees facing Bioinformatics Software
developers in the future. The second Keynote address was delivered by
[Hilmar Lapp](Hilmar_Lapp "wikilink"), Open Bio Foundation
Parliamentarian. He explained the exciting changes that the O\|B\|F was
undergoing in transitioning to a more active not-for-profit
organization, and invited BOSC attendees to become involved with the
foundation in ways that were not available to them before. Over the
course of two days, attendees were provided a wealth of information from
15 excellent 20-minute presentations selected from a very competitive
pool of applicants, and 17 lightning talks, speaking on a broad array of
topics. Birds of a Feather groups then formed in the afternoon around a
variety of specific topics, such as the DAS2 specification, and the
various Bio\* tools.

#### BOSC 2006

The BOSC committee is already in the process of planning [BOSC
2006](BOSC_2006 "wikilink"), to be held in conjunction with [ISMB
2006](http://ismb2006.cbi.cnptia.embrapa.br/) in [Fortaleza,
Brazil](wp:Fortaleza,_Brazil "wikilink"). We are looking forward to a
great meeting.

## O\|B\|F Projects Reports

### BioJava

*Contributed by [Mark Schreiber](Mark_Schreiber "wikilink")*

#### Biojava in 2005

2005 saw an increasing amount of activity for biojava. The long awaited
[biojava1.4](http://www.biojava.org/download14.html) was finally
released in June which re-energised the project. A big spike in web
activity for the biojava web-site was observed shortly after the
release. Hits per day increased from about 6000 per day to about 10K per
day after the release. The binary (JAR) distribution of biojava 1.4 has
been downloaded more than 4000 times since it's release with a typical
month seeing about 700 downloads.

The new activity has also increased the traffic on the mailing list and
has prompted a jump in number of active developers. At the same time
career changes work pressures have meant a few of the original lead
developers have taken more back seat role. Fortunately, their Oracular
wisdom can still be heard from time to time drifting from the mists of
the ethernet.

During 2005 the [Biojava in
Anger](http://www.biojava.org/docs/bj_in_anger/index.htm) site remained
popular and saw a big increase in the number of tutorials available.
There are now 64 short tutorials which cover most of the questions
commonly asked in biojava.

#### New developments

The release of biojava1.4 also cleared the way for new developments to
begin in earnest. Two exciting new developments are the biojavax
extensions and the biojava structure package.

##### Biojavax

Biojavax is an API extension to biojava. It has been designed to extend
the core interfaces of biojava without breaking any of the old design.
Incompatability between versions has been a key problem with previous
biojava releases. The idea is to increase the functionality of the core
API, particularly in the areas of file parsing and data persistence. The
relationship between biojavax and biojava is best compared to the
relationship of javax and java. Javax extends, improves and sometimes
deprecates the java API without being essential or breaking old code.

The need for biojavax came about when Richard Holland and I were working
on a biojava / biosql model for the dengue virus database
[dengueinfo](http://www.dengueinfo.org/). We quickly deficiencies with
biojava's biosql interaction model. We also identified areas where
flatfile I/O could be improved. Some fixes were made to the code base
but we also decided that the biojava core interfaces and I/O model could
be usefully extended. We also redesigned the biosql mappings so that all
persistence and transactions with biosql are now handled seamlessly by
[Hibernate](http://www.hibernate.org/). Although still experimental, we
hope to have a preview release of biojava1.5 including biojavax by early
2006.

##### Biojava Structure Package

Beginning in biojava1.4 and continuing to develop is biojava's structure
package. The package is designed to allow the I/O of PDB files.
Additionally it contains an object model that describes molecular
structures and allows for powerful manipulation and transformation of
those structures. The main developer of the package is Andreas Prlic who
is using it to develop a DAS client for structures called
[SPICE](http://www.efamily.org.uk/software/dasclients/spice/).

#### What is planned for 2006?

One of the core goals is to role out biojava1.5 including the biojavax
APIs. Following that I would like to extend the work we have done with
Hibernate to make use of the [Spring
Framework](http://www.springframework.org/). The intended goal is to
make biojava able to act as the middleware and/ or data object layer of
an enterprise application.

Another area for development in 2006 will be improving biojava's
abilities in data integration and interaction with semantic web
technologies like [RDF](http://www.w3.org/RDF/) by building on code
developed by Matthew Pocock when he was experimenting with his bjv2 API.

### BioMOBY

*Contributed by [Mark Wilkinson](Mark_Wilkinson "wikilink")*

In 2005, Bio[Moby](Moby "wikilink") enjoyed its most successful year so
far! This was the year that it emerged from its adolescence as "just an
amusing prototype", to mature into a serious codebase with a rigorous
test suite, increasingly comprehensive documentation, and a formal RFC
procedure for code changes. The number of independent Moby Web Service
registries has grown to 5 (Canada, Germany, Spain, Australia, and the
Philippines), and the number of interoperable services in the primary
public registry at UBC in Vancouver exceeds 500. Powerful and intuitive
tooling for service providers and for end-users has also become
available in the past year, lowering the bar for participation and use,
and greatly enhancing the accessibility of the BioMoby platform for the
"newbie". The BioMoby community of core developers has doubled this
year, and we have continued the tradition of having face-to-face
developers meetings every 6 months to ensure that the project does not
stagnate. Moby continues to enjoy a strong base of financial support
from the original Genome Canada award, and from a strong and productive
collaboration with the UK-based myGrid project, in addition to the many
participating members worldwide who invest their own resources into
tooling and core code improvements. We predict that 2006 will be the
year that BioMoby truly appears on the biologist's radar and starts
making a difference to the lives of researchers around the world!

### BioPerl

*Contributed by [Brian Osborne](Brian_Osborne "wikilink")*

The last 2 years in [BioPerl](BioPerl "wikilink") have been
characterized by significant acceptance and use by the academic and
commercial communities. Up until 2003 roughly [100
papers](https://web.archive.org/web/20070202113842/http://www.bioperl.org/wiki/BioPerl_publications#2003 "wikilink")
were published referring to the BioPerl package. Since then more than
[200
articles](https://web.archive.org/web/20070202113842/http://www.bioperl.org/wiki/BioPerl_publications#2006 "wikilink")
have appeared that cite BioPerl, primarily in the areas of genome
annotation and database construction. These figures, and data on Web
site use, show a steady increase in the popularity of BioPerl.

On the development side there has been much work on standardizing
documentation and increased testing, a full "bug sweep", and a
developer's release, version 1.5. In addition some 100 new modules have
been added in the last 2 years, for a total of 816 modules and roughly
173,000 lines of code.

On the community side a small group of dedicated supporters continued to
man the bioperl-l mailing list, which receives a steady stream of
queries. The most exciting news in this area is the new Wiki-based
BioPerl site which has been created in the last few months and will be
released in January 2006.

### Biopython

*Contributed by Iddo Friedberg [1](http://iddo-friedberg.org)*

Biopython [2](http://biopython.org) has had two releases in 2005, both
comprising of major additions to the code base. With 518 members
subscribed to the general mailing list, and 210 on the developers list,
Biopython has grown to become an important tool for the computational
biology community. Traffic on the developers list is high, with
contributions and patches submitted on a weekly basis. Currently the
project comprises of some 237,000 lines of code.

One of Python's [3](http://python.org) advantages is its ease of use and
mild learning curve, which makes it an ideal language for life
scientists who wish to program. However, Biopython's documentation, as
in many voluntary collaborative projects, has sorely been lagging behind
development. Thanks to efforts made by a few of our members, the
documentation basis has been greatly improved. We see the impact of this
in the mailing list, where many emails start with a variation of "I am
new to programming and to Python, and I have been using Biopython so far
and it is great! I just have one problem..." (We sometimes even manage
to help with that one problem). Ease of use has also made Biopython a
tool of choice for teaching Bioinformatics
[4](http://biopython.org/documentation/).

Biopython's ease of use does not mean it is a beginner's tool only.
Biopython is very comprehensive, having parsers for all major sequence
formats; mmCIF and PDB parsers for structures; pairwise and multiple
sequence alignment suites; machine learning tools, and more. Most major
bioinformatics databases have an associated Biopython module.

About 20 new modules were added in 2005. Notable newcomers are an NCBI
XML parser, a BLAT parser, a MEME parser... For a full list please see
the release notes [5](http://biopython.org/).

Several projects which use Biopython in their code base are:

- Joined Assessment of Functional Annotation (JAFA)
  [6](http://jafa.burnham.org)
- Text mining tools at Stanford University
  [7](http://bionlp.stanford.edu/)
- The **TRA**ns**M**embrane-**P**rotein **L**abelling **E**nvironment
  from BioDec [8](http://www.biodec.com/products)
- The upcoming Schneider suite [9](http://schneider.sourceforge.net/)
- A Google homepage script for calculating oligo melting temperatures:
  [10](http://www.bioinformatica.info/modules.php?op=modload&name=News&file=article&sid=301&mode=thread&order=0&thold=0)

Many thanks to all the contributors, too numerous to be mentioned here
[11](http://biopython.org/participants/). The 2005 releases were managed
by Iddo Friedberg[12](http://iddo-friedberg.org) (1.40 beta) and Michiel
de Hoon [13](http://bonsai.ims.u-tokyo.ac.jp/~mdehoon/) (1.41).

### BioSQL

*Contributed by Hilmar Lapp*

BioSQL is a generic relational model for storing biological sequences,
their features and annotation, and terms belonging to an ontology or
controlled vocabulary. The
[model](http://cvs.open-bio.org/cgi-bin/viewcvs/viewcvs.cgi/*checkout*/biosql-schema/doc/biosql-ERD.pdf?content-type=application/pdf)
imposes a unifying view on data sources as diverse as UniProt, GenBank,
Unigene, or LocusLink (or Entrez Gene). BioSQL is the [designated
persistence
API](http://open-bio.org/bosc2003/slides/Persistent_Bioperl_BOSC03.pdf)
between the Bio\* toolkits.

Originally created by [Ewan Birney](Ewan_Birney "wikilink") in 2001 to
de/serialize [BioPerl](https://bioperl.org "wikilink") sequence objects,
the present revision of the BioSQL schema is primarily the result of a
major review of the model by [Hilmar Lapp](Hilmar_Lapp "wikilink") and
[Aaron Mackey](bp:Aaron_Mackey "wikilink") at the Singapore Hackathon in
2003. Except for very minor changes, the model has essentially been
stable since then and will be named 1.0 upon official release. Several
post-1.0 extensions have already been discussed.

BioSQL is being used at multiple places worldwide, both academic and
commercial. It has been used as a component in several published
scientific works; a [Google Scholar
search](http://scholar.google.com/scholar?q=biosql) returns 30 hits. The
schema is fully supported by object-relational bridges for BioPerl
([Bioperl-db](bp:Bioperl_db "wikilink")) and Biojava (Biojavax).
Biopython and Bioruby support BioSQL for storing and retrieving sequence
objects, but don't fully leverage the ontology model. The release of the
1.0 version of the model is imminent, and an article describing the
model and its strengths is in preparation. Both will hopefully further
increase its consideration and adoption by developers and scientists in
the life science field.

Contact: The project home page is at <http://www.biosql.org>. The
mailing list is biosql-l@open-bio.org.

### BlipKit

*Contributed by [Chris Mungall](Chris_Mungall "wikilink")*

Blipkit (Biological Logic Programming Knowledge Integration Kit), aka
Blip, aka BioProlog, is a new addition to the OBF fold. Blip is an
integrated application programming library and a lightweight deductive
database system, and contains modules and schemas for representing and
using various biological and biomedical datatypes, such as sequence
features, phenotypes, pathways and phylogenies/species taxonomies. Blip
also has strong support for ontologies (both OBO and OWL).

Some end user scripts and applications are provided, including an AmiGO
clone. The current software is in alpha, early adopters are encouraged
to view:

<http://www.blipkit.org>

or the alternate url:

<http://www.bioprolog.org>

### CGL

*Contributed by [Mark Yandell](https://www.yandell-lab.org/ "wikilink")*

#### About CGL: the Comparative Genomics Library

[CGL](bp:CGL "wikilink") is an open source software library for
comparative genomics using genome annotations. The library is designed
to employ the contents of genome-annotation databases for purposes of
large-scale inquiries into the structure, function and evolution of
genes. To facilitate these analyses, CGL provides three core
functionalities. First, CGL can convert the annotations of many
different providers into a single standardized format (Chaos.xml); thus
the software can be used to assemble very large repositories of
annotations that encompass the contents of multiple genome databases.
Second, the library extends the bioperl HSP objects so that information
about annotated gene-structures is mapped to sequence alignments.
Finally, CGL can make use of existing annotations to in extract
information about gene structure from unannotated, partially assembled
genomes. For more information downloading and using CGL go
[www.yandell-lab.org/cgl](http://www.yandell-lab.org/cgl).

#### Current Release

Get the latest release of CGL from
[www.yandell-lab.org/cgl](http://www.yandell-lab.org/cgl).

Have a look at the main reference for CGL: Large-Scale Trends in the
Evolution of Gene Structures within 11 Animal Genomes [Mark
Yandell](https://www.yandell-lab.org/ "wikilink"), [Chris J.
Mungall](Chris_Mungall "wikilink"), Chris Smith, Simon Prochnik , Joshua
Kaminker, George Hartzell, [Suzanna Lewis](bp:Suzanna_Lewis "wikilink")
and Gerald M. Rubin. *In press* [PloS Computational
Biology](http://compbiol.plosjournals.org).

#### Contact us

General questions and comments about CGL should be directed to
[myandell-at-fruitfly.org](mailto:myandell_AT_fruitfly.org).

### DAS

[DAS](DAS "wikilink")

### GMOD

*Contributed by [Scott Cain](Scott_Cain "wikilink")*

The Generic Model Organism Database ([GMOD](GMOD "wikilink")) Project is
a largely open source project to develop a complete set of software for
creating and administering a model organism database. Components of this
project include genome visualization and editing tools, literature
curation tools, a robust database schema (known as Chado), and a generic
web front end. Several established model organism databases contribute
to the project, including WormBase, the [Saccharomyces Genome
Database](http://www.yeastgenome.org),
[FlyBase](http://www.flybase.net), [Gramene](http://www.gramene.org),
[TAIR](http://www.arabidopsis.org), the [Rat Genome
Database](http://rgd.mcw.edu/), and [EcoCyc](http://ecocyc.org/). Many
components of GMOD rely on [BioPerl](BioPerl "wikilink"), including one
of the "flagship" projects, the [Generic Genome Browser
(GBrowse)](Gbrowse "wikilink"), the widely adopted, web-based genome
feature visualizer. Over 150 organizations have adopted some tools from
GMOD.

#### Chado

Chado is a relational schema for model organisms designed around the
principles of modularity and extensibility via ontologies. The sequence
module lies at the core of the schema, and is used for representing
genomic features, their relationships and properties. In 2005 the
phylogeny module was added, and the genetics and phenotypes modules were
put into use by [FlyBase](http://www.flybase.org/).

*add stuff here from Scott Cain about chado, including a few adopting
orgs, like [TIGR](http://www.tigr.org/)
[dictyBase](http://www.dictybase.org/) and
[ParameciumDB](http://paramecium.cgm.cnrs-gif.fr/db/index).
[NESCENT](http://www.nescent.org/) are considering Chado for
evolutionary model organisms*

### PISE

*Contributed by Catherine Letondal*

[PISE](PISE "wikilink")

[Pise](http://www.pasteur.fr/recherche/unites/sis/Pise/) is an interface
generator for programs running under Unix. More precisely, it is a
software system which, given an XML description of a program's
parameters, generates source code for a user interface, as a component
of a system where the user can easily chain programs by pull-down menus.
A perl/[BioPerl](BioPerl "wikilink") API generator has also been
developed as well as a Python/[BioPython](BioPython "wikilink") API.

About 300 molecular biology programs have been defined under Pise,
including various sequence analysis, phylogeny, alignment, structural
analysis (RNA, secondary and tertiary structure) and gene prediction
programs. Pise has been in production for more than 8 years at the
[Pasteur Institute](http://www.pasteur.fr) (about 1500 submitted jobs a
day during the last year)
([bioweb.pasteur.fr](http://bioweb.pasteur.fr/)). The whole system, e.g
generators and the complete set of already defined interfaces is also
installed in several other sites, namely for interfacing
[EMBOSS](EMBOSS "wikilink") programs. Other users have developed new
programs' interfaces (in genetic analysis, primer design, and imaging
analysis). We are also aware of projects for building a new GUI
generator.

The project is now evolving towards a rewritten version, called Mobyle.
Mobyle is programmed in Python in a more robust and maintainable way. It
extends the wrapping mechanism to Web servers and Web services (mainly
using Biomoby). The web portal will provide more advanced navigation
features, enabling the user to search for services or re-use uploaded
data and parameterizing. See \[1\] for a more detailed description.

\[1\] B.Neron, P. Tuffery, C.Letondal (2005) [Mobyle: a Web portal
framework for bioinformatics
analyses](http://www.pasteur.fr/~letondal/Mobyle/neron_nettab.pdf),
poster presented at NETTAB 2005.

------------------------------------------------------------------------

*Newsletter edited by [Jason Stajich](Jason_Stajich "wikilink")*
