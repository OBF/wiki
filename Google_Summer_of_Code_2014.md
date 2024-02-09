---
title: Google Summer of Code 2014
permalink: Google_Summer_of_Code_2014
layout: wiki
---

## GSoC 2014

The Open Bioinformatics Foundation has been accepted as a mentoring
organization for Google Summer of Code 2014, with 6 student projects
funded!

## 2014 Student Projects

### Sarah Berkemer

Mentored by Christian Höner zu Siederdissen and Ketil Malde (BioHaskell)

- Project: "High-performance Transalign algorithm in Haskell"
- Blog: <http://biohaskell.org/GSoC_blog>
- Source code: <https://github.com/bsarah/transalign>

### Loris Cro

Mentored by Francesco Strozzi and Raoul Bonnal (BioRuby)

- Project: "An ultra-fast scalable RESTful API to query large numbers of
  VCF datapoints"
- Blog: <http://kappaloris.github.io/GSoC-2014-OBF/>
- Source code: <https://github.com/kappaloris/GSoC-2014-OBF>

### Victor Kofia

Mentored by Sarah Keating and Alex Thomas (JSBML)

- Project: "Redesign the implementation of mathematical formulas in
  JSBML"
- Blog: <http://kofiav.blogspot.ca/>
- Source code:
  <http://svn.code.sf.net/p/jsbml/code/trunk/core/src/org/sbml/jsbml/math/>

### Evan Parker

Mentored by Wibowo Arindrarto and Peter Cock (BioPython)

- Project: "Addition of a lazy-loading sequence parser to Biopython’s
  SeqIO package"
- Blog: <http://evanaparker.com/>
- Source code: <https://github.com/eparker05/biopython/tree/lazy-load>

### Ibrahim Vazirabad

Mentored by Andreas Dräger and Alex Thomas (JSBML)

- Project: "Improving the Plug-in interface for CellDesigner"
- Blog: <http://jsbmlcelldesigner2014.blogspot.com/>
- Source code: <http://sourceforge.net/projects/jsbml/>

### Leandro Watanabe

Mentored by Nicolas Rodriguez and Chris Myers (JSBML)

- Project: "Dynamic Modeling of Cellular Populations via arrays in
  JSBML"
- Blog: <http://lhwatanabe.blogspot.com>
- Source code: <http://sourceforge.net/projects/jsbml/> or
  <http://svn.code.sf.net/p/jsbml/code/trunk/extensions/arrays/>

## 2014 Projects Idea

The details of each of our project ideas are listed below, including
potential mentors. Interested mentors and students should subscribe to
the OBF/GSoC [mailing
list](http://lists.open-bio.org/mailman/listinfo/gsoc) and announce
their interest.

See the main OBF [Google Summer of
Code](Google_Summer_of_Code "wikilink") page for more information about
the GSoC program and additional ways to get in touch with us.

### Cross-project ideas

OBF is an umbrella organization which represents many different
programming languages used in
[bioinformatics](http://en.wikipedia.org/wiki/Bioinformatics). In
addition to working with each of the "Bio\*" projects (listed below),
this year we are also accepting a category of "cross-project" ideas that
cover multiple programming languages or projects. These collaborative
ideas are broadly defined and can be thought of as "unfinished" —
interested students should adapt the ideas to their own strengths and
goals, and are responsible for the quality of the final proposed idea in
their application.

**Feel free to propose your own entirely new idea**. You can also draw
ideas from [Genome Informatics
(GMOD)](http://gmod.org/wiki/GSoC#2014_Project_Ideas) and the [National
Evolutionary Synthesis Center
(NESCent)](http://informatics.nescent.org/wiki/Phyloinformatics_Summer_of_Code_2014).

#### Language APIs for the Systems Biology Markup Language (SBML) through the JVM

Rationale  
The standard Java implementation of SBML,
[JSBML](http://sbml.org/GSoC2014), is used as a parser for various
Java-based systems biology applications. This fulfills one niche, but
the versatility of the JVM can be utilized to employ JSBML as a parser
for systems biology applications that are written in other languages.
Also, JSBML undergoes an active community effort to be up-to-date with
current SBML standards.

<!-- -->

Approach  
This project will aim to present language APIs for languages that may
want to employ the SBML structure without building a parser from
scratch. Matlab, Mathematica, and Python APIs will be the focus for this
project.

<!-- -->

Languages and skill  
Java, optional: Matlab, Python, (other language)

<!-- -->

Mentors  
Andreas Dräger, Alex Thomas

#### [WormBase: data visualization](http://gmod.org/wiki/GSoC#WormBase:_data_visualization)

Rationale  
[WormBase](http://www.wormbase.org) is a central data repository
supporting the nematode research community. There are several areas of
improvement for data visualization on the website, including some key
points raised by the WormBase community.

<!-- -->

Approach  
Here are a couple requests we've received from the community, but we are
open to other ideas:

- Create a chromosome map tool - allow users to input and visualize the
  position of genetic loci. (See [community request
  \#1103](https://github.com/WormBase/website/issues/1103))
- Create a central dogma view to tie together our gene/protein/sequence
  pages. (See [community request
  \#557](https://bitbucket.org/tharris/wormbase/issue/557/add-central-dogma-nav-to-overview))

The website's back-end is written in Perl, using some BioPerl as well as
custom code. If you do significant work on the back-end, this could lead
to or involve BioPerl improvements.

<!-- -->

Languages and skills  
Front-end: Javascript, HTML5, JS graphical library of your choice (e.g.
D3). Back-end: some Perl, including BioPerl.

<!-- -->

Mentor(s)  
Abigail Cabunoc \<abigail.cabunoc@oicr.on.ca\>, others welcome

#### Improve SegAnnDB interactive genomic segmentation web app

Rationale  
[SegAnnDB](http://bioviz.rocq.inria.fr) is an open-source web site for
interactive genomic segmentation of DNA copy number profiles, [published
in
Bioinformatics](http://bioinformatics.oxfordjournals.org/content/early/2014/02/03/bioinformatics.btu072.short).
It combines previous work on data visualization, computer vision, and
machine learning into a web site that uses annotated regions to build a
user-specific segmentation model. YouTube videos explain how it works:
[basic annotation](https://www.youtube.com/watch?v=BuB5RNASHjU),
[annotating and exporting high-density
profiles](https://www.youtube.com/watch?v=al0kk1JWsr0). The goal of this
project is to add features to SegAnnDB.

<!-- -->

Approach  
The ideal student project would propose to

- Add social features for sharing annotations. SegAnnDB currently lets a
  user login using Mozilla Persona and then add user-specific
  annotations. These annotations are currently only accessible to the
  user that creates them, but it would be nice to be able to share them
  with others. For example, Alice annotates some data then types the
  email address of her friend Bob into a web form. Bob then receives an
  email with a web link where he can view Alice's annoatations.
- Add adminstrative features. SegAnnDB uses BerkeleyDB, which is very
  fast but makes updating and deleting profiles a bit tricky. I have
  started writing a view (plotter.views.delete_profiles) for profile
  deletion along with some database support (plotter.db.Profile.delete).
- Add unit tests using [Pyramid
  recommendations](http://docs.pylonsproject.org/en/latest/community/testing.html),
  for example when a profile is processed (plotter.db.Profile.process)
  test for presence of objects in the database, and then when the
  profile is deleted, check for deletion of relvant objects and files
  (PNG scatterplots, probes.bedGraph.gz data).
- Add support for browsers that do not render large PNG images. SegAnnDB
  uses very large PNGs to efficiently visualize DNA copy number
  profiles, but these are not supported by all browsers and [you can
  test your browser's support on this web
  page](http://sugiyama-www.cs.titech.ac.jp/~toby/images/).
- Attempt integration with Galaxy, possibly as a [Visualization
  Plugin](https://wiki.galaxyproject.org/VisualizationsRegistry).
- Integration of [SegAnnot and PrunedDP extension
  modules](https://r-forge.r-project.org/scm/viewvc.php/python/?root=segannot)
  into BioPython.

Required skills  
JavaScript and Python. Experience with [D3](http://d3js.org/) and
[Pyramid](http://www.pylonsproject.org/projects/pyramid/about) web
framework a plus.

<!-- -->

Code  
SegAnnDB is implemented as a Pyramid web app with a D3/JavaScript
interface. Download the source code with

`svn checkout svn://scm.gforge.inria.fr/svnroot/breakpoints/webapp/pyramid SegAnnDB`

and then check 00_INSTALL.sh for installation instructions, and email me
if anything is unclear.

Mentors: Toby Dylan Hocking tdhock5@gmail.com plus anyone else with experience with D3/Pyramid is welcome to help!  

#### Integrate basic biological data analysis capabilities in fastR (Java/R)

Rationale  
R is a free software programming language and software environment for
statistical computing and graphics. The R language is widely used among
statisticians and data miners for developing statistical software and
data analysis. Despite this, R is hard to mantain and evolve, lacks
portability features and is characterized by low performance. The FastR
project
(http://www.oracle.com/technetwork/java/jvmls2013vitek-2013524.pdf) aims
to rethink how to implement R, by leveraging well tested technologies to
build a high performance VM. FastR is an implementation of the R
programming language in Java using AST interpretation and specialisation
for improved performance. The implementation has been extended to
support JIT compilation, leading to performance improvements.

The fastR project has been presented to the useR! conference 2013, and
it is now being actively developed at
<https://bitbucket.org/allr/fastr>.

Approach  
The goal of this project would be to carry on the FastR development by
expanding the set of supported R data types, possibly integrating some
basic functionalities from Bioconductor which will be extended in the
future. The strength of this approach lies in the possibility for Java
users to access the vast R ecosystem, and to expand further the
inter-operability of R packages and workflows by using other languages
built on Java, like JRuby and Jython.

<!-- -->

Required skills  
Moderate technical difficulty, an interest in statistical problem
solving is a plus but not essential. This project requires mid/advanced
Java programming skills

<!-- -->

Reference to other projects: BioJava, R, BioRuby, Jruby, Jython  

<!-- -->

Mentors: Jan Vitek, Alberto Arrigoni \[arrigonialberto86@gmail.com\]  

#### BioInterchange: Convert and Exchange Biological File Formants using RESTful web service

Rationale  
[BioInterchange](http://www.biointerchange.org/index.html) Interchange
data using the Resource Description Framework (RDF) and let
BioInterchange automagically create RDF triples from your TSV, XML,
GFF3, GVF, Newick and other files common in Bioinformatics.
BioInterchange helps you transform your data sets into linked data for
sharing and data integration via command line, web-service, or API.
BioInterchange was conceived and designed during NBDC/DBCLS's
[BioHackathon 2012](http://2012.biohackathon.org/). Architecture and RDF
serialization implementations were provided by Joachim Baran, Geraint
Duck provided JSON and XML deserialization implementations and
contributed to architecture decisions, guidance on ontology use and
applications were given by Kevin B. Cohen and Michel Dumontier, where
Michel brought forward and extended the Semanticscience Integrated
Ontology (SIO). Jin-Dong Kim helped to define ontology relationships for
RDFizing DBCLS' PubAnnotation category annotations. The main idea is to
have a central service with can be used as a validator and as
interchange service for different languages.

<!-- -->

Approach  
The project will identify the most common and used file formants for all
the currently used language under OBF and will design a RESTful API and
will project an implementation for all the supported languages.
BioInterchange was developed with Ruby but the scope of the project is
to have an agnostic system which let use implement a converter using the
best language for that functionality. It expected to have a high traffic
for the service so an appropriate refactoring or reimplementation using
parallel techniques or languages devoted to parallel programming would
be possible.

<!-- -->

Difficulty and needed skills  
The project is mid / high difficulty, aimed at talented students.
Previous knowledge of Ruby or other scripting language is preferred and
flexibility in learning other languages is required.

The project requires  
Knowledge of advanced programming languages and meta-programming and
some concept in parallelizing and web services design.

<!-- -->

Mentors  
Raoul J.P. Bonnal, Francesco Strozzi, Toshiaki Katayama, Joachim Baran

#### bionode - A Node.js JavaScript library for client and server side bioinformatics

Rationale  
During the development of a web front-end or software with a
web-interface, it often becomes clear that a component implemented for
the server-side must be performed on the client side, or vice-versa.
This generally requires functionalities implemented in one language to
be reimplemented in another. Recent developments in Javascript make this
unnecessary. Indeed, JavaScript has become a “write once run everywhere”
full stack programming language that can be executed in the browser as
well as on the server (thanks to Node.js). The web-development community
is enthusiastically embracing this technology. In the last year, Node.js
modules increased [2.6-fold to a total of
61656](http://modulecounts.com). The average growth rate is 175 modules
per day, which means that it will quickly surpass Java (71906) and
Ruby (71446) having already surpassed all the other languages (e.g.,
Perl: 29097; Python: 40455).

<!-- -->

  
Consistent with this, web applications for visualizing or interacting
with biological data increasingly rely on javascript (e.g.
[jBrowse](http://jbrowse.org),
[WebApollo](http://apollo.berkeleybop.org),
[Biodalliance](http://biodalliance.org), etc). Surprisingly however, no
generic javascript bioinformatics library yet exists, leading
independent projects to redundantly implement basic functionality. Here,
we propose to develop bionode a core javascript library for handling and
analyzing bioinformatics data - mirroring the core functionality of
established bio\* libraries (e.g. bioperl, bioruby).

<!-- -->

  
This will be done in close collaboration with the developers of
[BioJS](http://rostlab.org/services/biojs/gsoc.html) (who build reusable
components for visualization of biological data) and of
[WebApollo](http://apollo.berkeleybop.org)/[Afra](http://github.com/yeban/afra)
(a gene prediction curation software) for immediate short-term
applications. Importantly, we expect the long-term interest for a
bioinformatics javascript library to be huge.

<!-- -->

Approach  
We already seeded this project: [bionode](http://bionode.io) is a
Node.js module with some bioinformatics methods that work on the client
and server side.

Under the supervision of the mentor(s), the GSoC student will add more
methods/algorithms to the bionode project. The student could take
inspiration from other similar libraries in other programming languages,
such as [bioperl](http://bioperl.org/wiki/Main_Page) or
[bioruby](http://bioruby.open-bio.org/wiki). Methods for input/output
and wrangling basic data types should be given a higher priority at the
beginning of this projects. For example, implementing some of the
functions of [biopython.SeqIO](http://biopython.org/wiki/SeqIO) could be
a project. Another source for inspiration could come from Massive Open
Online Course, such as the [“Bioinformatics
Algorithms”](http://www.coursera.org/course/bioinformatics) from the
University of California, San Diego.

<!-- -->

Challenges  
Methods provided should be able to run on a server environment (via
Node.js) or browser environment (via webpack or browserify). Thus, the
module pattern used should be the one used by Node.js (CommonJS).

Good programming practices should be used, the code should be clear,
well documented and unit tested. Furthermore, relevant examples should
be provided for novice users (i.e. biologists who are just learning to
program).

<!-- -->

Difficulty and needed skills  
The student should ideally have an very good knowledge of JavaScript and
basic knowledge of bioinformatics/biology.

Experience using GitHub for collaboration would be a big plus.

<!-- -->

Mentors  
Bruno Vieira ([@bmpvieira](http://twitter.com/bmpvieira))
\<<mail@bmpvieira.com>\>, Yannick Wurm
([@yannick\_\_](http://twitter.com/yannick__))

### [BioPerl](http://bioperl.org/wiki/Google_Summer_of_Code)

<img src="BioPerl_logo_tiny.jpg" title="BioPerl logo" />

- [Mailing lists](https://bioperl.org/Support "wikilink")
- IRC: `#bioperl` on [Freenode](http://freenode.net)
- [Information for new developers](bp:Becoming_a_developer "wikilink")
- Source code browser for
  [bioperl-live](https://github.com/bioperl/bioperl-live) (the main
  BioPerl code base), and [all BioPerl
  sub-projects](https://github.com/bioperl)
- [Priority list](bp:Project_priority_list "wikilink") of things that
  need work, as another source for student-conceived project ideas

#### [NGS-friendly BioPerl code](http://bioperl.org/wiki/Google_Summer_of_Code#NGS-friendly_BioPerl_code)

Rationale : BioPerl is known to be slow re: any data sets, but particularly when dealing with very large data (e.g. anything related to NGS analysis. Can we make it better? Where should we focus our efforts?  

<!-- -->

Approach : Under the supervision of their mentor(s), the GSoC student will:  

:\* Benchmark bottlenecks that lead to loss in performance for NGS
analyses

:\* Refactor old classes or develop new optimized code for NGS analysis

Challenges : This can be a self-contained project, but will require a lot of discussion on what areas to focus on.  

<!-- -->

Difficulty and needed skills : easy to hard, depending on student's familiarity with the tools to be used. Student will need:  

:\* excellent Perl programming skills, including familiarity with NGS
datasets

\* knowledge of modern Perl practices.  

<!-- -->

Mentors : Chris Fields, others?  

#### \[<http://bioperl.org/wiki/Google_Summer_of_Code#Convert_BioPerl-DB_to_DBIx>::Class Convert BioPerl-DB to use DBIx::Class\]

Rationale : Bioperl-db (the BioPerl bindings to BioSQL) in essence constitute a self-made ORM, invented at a time when DBIx::Class didn't exist yet. As such, it has some advantages (if you are willing to count overly clever features to be counted in this category), but arguably many more disadvantages, chief among them being the unsustainably small (you could also say non-existent) developer community supporting it, and the fact that DBIx::Class now has existed for years, and is fairly mature. So, rewriting Bioperl-db with a DBIx::Class (or another well-supported generic ORM) would stand to make a considerable impact on our ability to further develop Bioperl's relational storage capabilities, as well as BioSQL itself.  

<!-- -->

Approach : Under the supervision of their mentor(s), the GSoC student will:  

:\* Start working on conversion of BioPerl-DB classes to using
DBIx::Class

:\* write additional tests and improve documentation as needed

Challenges : BioPerl-DB is self-contained; this may require looking at the BioSQL schema and determining whether there are specific areas that need the most focus.  

<!-- -->

Difficulty and needed skills : easy to hard, depending on student's familiarity with the tools to be used. Student will need:  

:\* excellent Perl programming skills, including familiarity with:

:\*\* DBIx::Class

Mentors : Hilmar Lapp, others?  

#### [Major BioPerl Reorganization (Part II)](http://bioperl.org/wiki/Google_Summer_of_Code#Major_BioPerl_Reorganization.2C_part_2)

Rationale : The initial run at this project [had some success](http://bioperl.org/wiki/Google_Summer_of_Code#Major_BioPerl_reorganization), but more work needs to be done. The final goal of this project is to find and break out as many well-defined subsections of BioPerl as possible, releasing them to CPAN along the way.  

<!-- -->

Approach : Under the supervision of their mentor(s), the GSoC student will:  

:\* break current thousand-module monolithic distributions into smaller,
more manageable pieces

:\* improve characterization of dependencies

:\* improve build and testing systems for new distributions

:\* write additional tests and improve documentation as needed for the
reorganization

Challenges : BioPerl contains nearly 2000 modules, with very complex relationships between them.  

<!-- -->

Difficulty and needed skills : easy to hard, depending on student's familiarity with the tools to be used. Student will need:  

:\* excellent Perl programming skills, including familiarity with:

:\*\* testing (`prove`, `TAP::Harness`)

:\*\* module authoring (`Module::Build`,`Dist::Zilla`,PAUSE)

:\* good knowledge of command-line text-processing tools like `ack`,
`grep`, and Perl one-liners.

:\* version control systems (BioPerl uses [git](http://git-scm.com)).

Mentors : Chris Fields, others?  

#### [Perl Run Wrappers for External Programs in a Flash](http://bioperl.org/wiki/Google_Summer_of_Code#Perl_Run_Wrappers_for_External_Programs_in_a_Flash)

Rationale : BioPerl has a long tradition of providing wrapper objects for running external programs and parsing their output, mainly through the distribution called [bioperl-run](http://bioperl.org/wiki/Bioperl-run). Wrappers make it relatively easy to process data in highly customizable pipelines with the benefits of BioPerl objects and I/O. They also help to standardize the interfaces to typically idiosyncratic open-source utilities, reducing the burden on the developer. With new bioinformatics tools being released almost daily, however, it can be difficult for the BioPerl regulars to maintain a stable of run wrappers for the latest and greatest tools. Even harder is making the wrapper interfaces themselves conform to a standard API that users can count on.  

<!-- -->

Possible approaches:  

1.  Integrate Galaxy's tool configuration file format in a pluggable way
    for developing a generic wrapper application.
2.  Improve/tighten/extend the `Bio::Tools::Run::WrapperBase` and
    `Bio::Tools::Run::WrapperBase::CommandExts` system for very general
    run wrappers, making them work robustly with the new
    `Bio::Tools::WrapperMaker` module currently under development. The
    goal will be to get these modules ready for release into the trunk.
3.  Are there any shortcomings to current schemes, such as Galaxy's or
    EMBOSS's acd format, that could be addressed with a newer schema?

See [HOWTO:Wrappers](http://bioperl.org/wiki/HOWTO:Wrappers) and the
above module documentation for more details.

Difficulty and needed skills : Medium. The student should understand or be willing to work hard at understanding BioPerl object-oriented style. Some familiarity with [XML](wp:XML "wikilink") and [XML Schema](wp:XML_Schema "wikilink") will help in getting up to speed. An interest in playing with new open-source bioinformatics tools, especially those for managing next-generation sequence assembly, would also be valuable.  

<!-- -->

Mentors : [ Chris Fields](User%3ACjfields "wikilink")  

#### [Lightweight BioPerl modules](http://bioperl.org/wiki/Google_Summer_of_Code#Lightweight.2FLazy_BioPerl_Classes)

Rationale : Many current BioPerl classes are implemented in a greedy or heavy way, where all information is pulled into memory as objects. For instance, the current `Bio::Seq` implementation is the primary bottleneck for sequence parsing speed and can take up a ton of memory, particularly with whole-genome information and next-generation sequencing information. Storing the data in memory in a simple data structure and generating the objects lazily could help with speed. Alternatively, storing the data in a persistent manner would also help with memory issues, with the obvious trade-off for speed but having the nice side-benefit of consistent and possibly persistent ways of handling data.  

<!-- -->

Approach : Implement a `Bio::Seq`/`Bio::PrimarySeq` class (or other commonly-used BioPerl classes) that can deal with very large datasets in a memory-efficient manner. Implement at least one corresponding parser that can either parse records lazily (akin to an XML pull parser) or create lightweight objects. These could be considered two projects but they are interrelated (lightweight objects could have many different backends, including lazy parsing), so development should proceed with this in mind.  

<!-- -->

Difficulty and needed skills : medium to hard. Student should have an excellent command of Perl and data structures, experience with persistent storage mechanisms (such as a SQL-based RDBMS, CouchDB, etc), and some familiarity with parsing methodologies.  

<!-- -->

Prior art : Jason Stajich has started a SQLite-based lightweight `Bio::Tree::Tree` implementation on [a GitHub branch](http://github.com/bioperl/bioperl-live/tree/topic/tree_dbsqlite_memoryfix) at the recent GMOD Evolutionary Biology Hackathon at NESCent in Fall 2010.  

<!-- -->

Mentors : Chris Fields  

#### [BioPerl 2.0 and beyond](http://bioperl.org/wiki/Google_Summer_of_Code#BioPerl_2.0_.28and_beyond.29)

Rationale : Design or reimplement BioPerl classes without API constraint, using Modern Perl tools or Perl 6.  

<!-- -->

Approach : Most BioPerl code is over 6 years old and doesn't take advantage of Modern Perl tools, such as new methods available in Perl 5.10 and 5.12, Moose/MooseX, DBIx::Class, Catalyst, and more. Furthermore, a viable Perl6 implementation, Rakudo, is currently available. This gives us an enormous opportunity to redesign fundamental aspects of BioPerl without the necessity for development hindered by a requirement for backwards compatibility.  

Two projects, Biome (Moose-based BioPerl) and BioPerl6 (Perl 6 BioPerl)
have already started but are in a very early stage. One could
participate in:

- IO implementations for object iteration, or Perl6 grammars for common
  formats
- Redesign of common BioPerl classes
- etc.

This is an area ripe for new student project ideas. The more focused the
better! Discussion is a must, either via IRC or email.

Difficulty : Project-dependent  

<!-- -->

Mentors : Chris Fields, Rob Buels  

#### \[<http://bioperl.org/wiki/Google_Summer_of_Code#Bio>::Assembly Bio::Assembly\]

Rationale  
Although progress was made in the 2010 project "Alignment Subsystem
Refactoring", continued refinement of AssemblyIO is still needed.

<!-- -->

Approach  
SAM or ACE files once imported should have similar handles and/or
methods.

<!-- -->

Difficulty and needed skills  
Medium. Proficiency in Perl, familiarity with assembly tools.

<!-- -->

Mentors  
To be determined.

#### [Semantic Web Support](http://bioperl.org/wiki/Google_Summer_of_Code#Semantic_Web_Support)

Rationale : There are great development opportunities in information discovery for bioinformatics using semantic web, specially thinking in the implementation of SPARQL queries for a "discoverable bio-cloud".  

<!-- -->

Approach : Previous efforts can be adopted and extended, such as resulting code from [BioHackathon 3](http://hackathon3.dbcls.jp/) and the code provided by [Expasy](http://dev.isb-sib.ch/projects/expasy-rdf/). Using the modules of the [Semantic Web with Perl community](http://www.perlrdf.org), built around \[<https://metacpan.org/module/RDF>::Trine RDF::Trine low-level API\]. There are two main areas to explore:  

1.  Parsers and converters from and to RDF, including IO modules for
    GenBank, EMBL, several XML specifications, et cetera.
2.  Storage and retrieval of information using SPARQL.

Difficulty and needed skills : Medium. Familiarity with SeqIO modules and Perl itself. The student should also be familiar with RDF format and the RDF triples concept for Semantic Web.  

<!-- -->

Mentors : To be determined. [Kjetil Kjernsmo](http://bioperl.org/wiki/User:Kjetilk) can help mentor students wishing to explore the RDF::Trine direction.  

### [BioJava](http://biojava.org/wiki/Google_Summer_of_Code) and JSBML

<img src="Biojava_logo_tiny.jpg" title="BioJava logo" />

- [BioJava developer mailing
  list](http://lists.open-bio.org/mailman/listinfo/biojava-dev)
- [JSBML developer mailing
  list](https://groups.google.com/forum/#!forum/jsbml-development)
- [BioJava modules](http://biojava.org/wiki/BioJava:Modules) as another
  source for student-conceived project ideas
- Source code for
  [biojava-live](http://code.open-bio.org/svnweb/index.cgi/biojava/browse/biojava-live/trunk)
  (the main BioJava code base) and [all BioJava
  sub-projects](http://code.open-bio.org/svnweb/index.cgi/biojava/)

For GSoC 2014, BioJava is partnering with the Systems Biology Markup
Language (SMBL) team to bring enhancements to JSBML, the standard Java
implementation of SBML, and bring SBML features to other Java-based
systems biology software. See [the SMBL
website](http://sbml.org/GSoC2014) for more ideas from the SBML team.

Students working on these projects will interact with both the BioJava
and JSBML communities, which overlap. Most development will happen on
the JSBML codebase, although BioJava is used as a supporting library for
some components.

#### Add support for Schema-based validation of SBML

Rationale  
SBML files need to be validated carefully to ensure that they conform to
the specification. Currently, the most complete implementation of SBML
validation is embodied in libSBML, although the rules of SBML validity
are defined in the SBML specification documents. It is possible to
validate SBML from JSBML using either the Online SBML Validator or a
Java package we provide for calling libSBML locally (i.e., without a
network connection) but we want to move toward capturing all of the
SBML's validity rules in schema languages.

<!-- -->

Approach  
Capture all of the SBML's validity rules in schema languages such as
RELAX NG and Schematron, then have both libSBML and JSBML (and any other
SBML-using system) use schema validation engines instead of hardcoded
validation. This will be especially important as more SBML Level 3
packages become implemented. We have already made great strides in
defining RELAX NG schemas for SBML Level 3, but we need to work on
providing the hooks in JSBML to using those schemas for validating SBML
files.

<!-- -->

Languages and skills  
Java, XML, RELAX NG, Schematron, SBML

<!-- -->

Mentors  
Sarah Keating, Andreas Dräger

#### Redesign the implementation of mathematical formulas in JSBML

Rationale  
JSBML uses the concept of abstract syntax trees to work with
mathematical expressions. At the moment, all different kinds of formulas
are implemented in one complex class.

<!-- -->

Approach  
This project should implement a math package for JSBML, in which all
different kinds of tree nodes that can occur in formulas (e.g., real
numbers or algebraic symbols such as 'plus' or 'minus') would be
represented with an own, specialized class. In this way, the handling of
formulas would be much more straightforward and even more efficient.

<!-- -->

Difficulty and skills  
Medium; proficient in Java

<!-- -->

Mentors  
Andreas Dräger, Alex Thomas, Sarah Keating

#### Implement support for the SBML Multistate/Multicomponent Species package

Rationale  
One of the many packages for SBML Level 3 is Multistate and
multicomponent species. This packages define constructs for models and
modelers to represent biochemical species that have internal structure
or state properties. These may involve molecules that have multiple
potential states, such as a protein that may be covalently modified, and
molecules that combine to form heterogeneous complexes located among
multiple compartments.

<!-- -->

Approach  
The JSBML team has already started implementation of the `multi`
package, but more needs to be done.

<!-- -->

Languages and skills  
Java, some exposure to biochemistry

<!-- -->

Mentors  
Nicolas Rodriguez, Nicolas Le Novère

#### Improve the plugin interface for CellDesigner

Rationale  
One of the most frequently used programs in computational systems
biology is [CellDesigner](http://www.celldesigner.org/). JSBML provides
an interface that facilitates the development of plugins for this
program. This interface has recently been revised and improved.

<!-- -->

Approach  
Test cases and plugins for CellDesigner are to be implemented in order
to make use of it and ensure its correct behavior. It is, for instance,
possible to use CellDesigner's complex canvas user interface to create
or manipulate biochemical networks and to conduct numerical computation.

<!-- -->

Languages and skills  
Java, some basic understanding of visualization algorithms

<!-- -->

Mentors  
Andreas Dräger

### [BioPython](https://biopython.org/wiki/Google_Summer_of_Code "wikilink")

<img src="Biopython_logo_tiny.png" title="Biopython logo" />

- [Mailing lists](https://biopython.org/wiki/Mailing_lists "wikilink")
- [Information for
  contributors](https://biopython.org/wiki/Contributing "wikilink")
- [ Source Code](https://biopython.org/wiki/SourceCode "wikilink")

#### [Indexing & Lazy-loading Sequence Parsers](http://biopython.org/wiki/Google_Summer_of_Code#Indexing_.26_Lazy-loading_Sequence_Parsers)

Rationale  
[Bio.SeqIO](https://biopython.org/wiki/SeqIO "wikilink")'s indexing
offers parsing on demand access to any sequence in a large file (or
collection of files on disk) as a <https://biopython.org/wiki/SeqRecord>
object. This works well when you have many small to medium sized
sequences/genomes. However, this is not ideal for large genomes or
chromosomes where only a sub-region may be needed. A lazy-loading parser
would delay reading the record until requested. For example, if region
*record\[3000:4000\]* is requested, then only those 1000 bases need to
be loaded from disk into memory, plus any features in that region. This
is how Biopython's <https://biopython.org/wiki/BioSQL> interface works.
Tools like tabix and samtools have demonstrated efficient co-ordinate
indexing which could be useful here.

Aside from being used via an index for random access, lazy-loading
parsers could be used when iterating over a file as well. This can
*potentially* offer speed ups for tasks where only a fraction of the
data is used. For example, if calculating the GC content of a collection
of genomes from GenBank, using Bio.SeqIO.parse(...) would currently
needlessly load and parse all the annotation and features. A lazy-parser
would only parse the sequence information.

Approach & Goals  
Useful features include:

- Internal indexing of multiple file formats, including FASTA and richly
  annotated sequence formats like GenBank/EMBL and GTF/GFF/GFF3.
- Full compatibility with existing SeqIO parsers which load everything
  into memory as a \`SeqRecord\` object.

Difficulty and needed skills  
Hard. Familiarity with the Biopython's existing sequence parsing
essential. Understanding of indexing large files will be vital.

Possible Mentors  
[Wibowo Arindrarto](https://github.com/bow), [Peter
Cock](https://github.com/peterjc/), others welcome

#### [Interactive GenomeDiagram Module](http://biopython.org/wiki/Google_Summer_of_Code#Interactive_GenomeDiagram_Module)

Rationale  
The GenomeDiagram genome/comparative genomics visualisation module
currently produces static images (bitmap format), or images with
relatively limited interactive capability such as click-throughs (.pdf,
.svg). This is fine for its original intent of producing
publication-quality graphics, but interactivity such as dynamic
formatting, data selection, and box-outs would greatly enhance the value
of the existing visualisations, and enable new uses.

Approach & Goals  
The [Bokeh](http://bokeh.pydata.org/) interactive visualisation library
uses the standalone [BokehJS](http://bokeh.pydata.org/dev_guide.html)
backend for in-browser visualisation. Targeting BokehJS with
GenomeDiagram ought to be possible.

Difficulty and needed skills  
Looks tricky to me. Introduction of BokehJS brings dependencies that may
not be desirable for Biopython. BokehJS is in Coffeescript - the Python
interface is not well documented. Familiarity with Javascript would be
very useful.

Possible Mentors  
[Leighton Pritchard](https://github.com/widdowquinn) though I'd be
learning as much as the student, so others very welcome.

### [BioRuby](http://bioruby.open-bio.org/wiki/Google_Summer_of_Code)

<img src="BioRuby_logo_tiny.png" title="BioRuby logo" />

- [Developers mailing
  list](http://lists.open-bio.org/mailman/listinfo/bioruby)
- [Source code](http://github.com/bioruby/bioruby/tree/master)
- IRC: `#bioruby` on [Freenode](http://freenode.net)

#### [An ultra-fast scalable RESTful API to query large numbers of genomic variations](http://bioruby.open-bio.org/wiki/Google_Summer_of_Code#An_ultra-fast_scalable_RESTful_API_to_query_large_numbers_of_genomic_variations)

Rationale  
VCF files are the typical output of genome resequencing projects
(http://www.1000genomes.org/node/101). They store the information on all
the mutations and variations
([SNPs](http://en.wikipedia.org/wiki/Single-nucleotide_polymorphism) and
[InDels](http://en.wikipedia.org/wiki/Indel)) that are found by
comparing the outputs of a
[NGS](http://en.wikipedia.org/wiki/DNA_sequencing#Next-generation_methods)
platform with a reference genome. These files are not incredibly large
(a typical uncompressed VCF file is few gigabytes) but they are full
with information on millions of positions in the genome where mutations
are found. Large resequencing projects can produce hundreds or thousands
of these files, one for each sample sequenced.

Existing tools (such as [VCFTools](http://vcftools.sourceforge.net) or
[BCFTools](http://samtools.sourceforge.net/samtools.shtml#4)) offer a
convenient way to access these files and extract or convert the
information present, but are limited in functionalities and speed when
more complex queries need to be performed on these data. With existing
tools it is very complicated, if not impossibile, to retrive information
when working on many VCF files and samples together to compare, for
instance, the variations found in 100 samples and extract all the
mutations that are present in 50 samples but are not present in the
other 50 and so on.

<!-- -->

Approach  
The project should develop a RESTful API to address the issues described
in the rationale and to allow users to manipulate and compare genomics
variation information for hundreds of samples. A database engine will be
required to store the information and to support the data mining.
Unstructured database engines such as noSQL databases or key-values
stores can all be valid alternatives to combine high-speed with data
flexibility. The decision on the best database engine to be used will be
discussed between the student and the mentors and within the OpenBio
community. Given the high amount of information that will need to be
processed by such an application, scalable and fast languages such as
JVM-based languages like Scala or JRuby will be a good choice. The
project should also take care of the deploy of such an API, by creating
a Ruby gem or a JAR that users can install and use right away with their
datasets.

<!-- -->

Difficulty and needed skills  
The project has an average difficulty and it is aimed at talented
students who wants to develop a fast API to address these problems.

The project requires  
Knowledge of advanced programming languages. Some experience and
knowledge of databases and data mining will help managing the
information of VCF files.

<!-- -->

Mentors  
Francesco Strozzi, Raoul J.P. Bonnal

### [BioHaskell](http://biohaskell.org/Google_Summer_of_Code)

:\* [Project website](http://biohaskell.org/)

:\* [Bioinformatics section on
HackageDB](http://hackage.haskell.org/packages/#cat:Bioinformatics)

#### [Optimizing transalign, a novel, very sensitive alignment method](http://biohaskell.org/Google_Summer_of_Code#Optimizing_transalign)

Rationale  
A method and implementation for more sensitive pairwise alignments was
recently developed and published (paper is
[here](http://dx.plos.org/10.1371/journal.pone.0054422), and a copy
[here](http://malde.org/~ketil/publications/Malde2013a.pdf)). The method
appears to be the best of its type -- if nothing else, check the SCOP
benchmark -- although it’s difficult to construct a good test case using
more complex methods (training sets for HMMs and whatnot). The current
implementation is in Haskell, and although it works correctly, it is a
bit slow, and more problematic, it consumes too much memory (so going
multi-threaded, although pretty easy, won’t be of any help).

<!-- -->

Approach  

<!-- -->

  
The goal is to make this into a more practical tool by reducing resource
requirements. A prospective student would either:

1.  Optimize the Haskell program, primarily to reduce memory footprint,
    and secondarily to make use of multi-CPU systems.
2.  Reimplement the algorithm (or parts of it) in a different language,
    and achieving the same as above.

  
Advantages of 1:

:\* Already have a working program, and the type system makes it easy to
refactor without introducing errors.

:\* Haskell supports lots of good multi-threading programming models
(like STM)

:\* The author of the method, Ketil, knows Haskell pretty well and will
mentor.

  
Disadvantages:

:\* Haskell has some good debugging tools, but they tend to work really
poorly for large memory (i.e. it takes a long time to generate profiles)

:\* Needs somebody with a bit (or a lot) of experience optimizing
Haskell, and good knowledge of high-perf libraries (like vector)

  
Advantages of 2:

:\* Easier to get a student with adequate skills.

:\* More predictable performance models in other languages.

:\* Easier to compile and install for many users.

  
Disadvantages:

:\* Ideally, should know enough Haskell to read and understand the code.

:\* Likely needs a co-mentor with knowledge of the language in question.

Difficulty and skills needed  
Medium to hard; Haskell proficiency and some knowledge of algorithm
development

<!-- -->

Mentor:  
Ketil Malde (ketil@malde.org)

### [Biocaml](http://biocaml.org)

:\* [Mailing List](https://groups.google.com/d/forum/biocaml)

#### Bioinformatics Js_of_ocaml Visualization Toolkit

Rationale  
[OCaml](http://ocaml.org) is a strong statically typed functional
programming language. Usually one does not consider such languages for
front-end development, but the Js_of_ocaml compiler is causing OCaml to
be more widely used for building websites.
[Js_of_ocaml](http://ocsigen.org/js_of_ocaml/) compiles OCaml code to
pure Javascript and the generated Javascript has [very good
performance](http://ocsigen.org/js_of_ocaml/manual/performances). On the
other hand, bioinformatics data analysis needs to be conducted by a
broader range of users, which requires more elegant user interfaces with
high quality data visualization.

<!-- -->

Approach  
Write an OCaml library that can be used to visualize large data sets
efficiently and interactively in the browser. The library should be
smart enough to work on the client side when possible, but make server
side calls when necessary. You may want to use
[Eliom](http://ocsigen.org/eliom/) for this purpose. You can connect to
parsers and data structures available in [Biocaml](http://biocaml.org)
as needed. As demonstration of success, it should be possible to create
genome visualizations like that of the [UCSC genome
browser](http://genome.ucsc.edu/cgi-bin/hgGateway) and protein
interaction networks like that of
[Cytoscape](http://www.cytoscape.org/).

<!-- -->

Difficulty and needed skills  

This project is for intermediate to advanced programmers. You will need
to be already familiar with OCaml (or closely related languages like F#
and Haskell) and have a basic understanding of Javascript and
client/server programming.

Mentor  
[Ashish Agarwal](http://ashishagarwal.org) \<agarwal1975@gmail.com\>
