---
title: BOSC 2006/Abstracts
permalink: BOSC_2006/Abstracts
layout: wiki
redirect_from:
 - Abstracts
---

## BioPostgres

D.S. Parker, Ph.D. UCLA

Friday August 4th, 9:00am

BioPostgres is a collection of modules that can be used to extend
PostgreSQL, the popular open-source database system, for bioinformatics
and computational biology. Each of the BioPostgres modules is intended
to be independent, and to be usable separately or in conjunction with
the others. Current modules include:

BLASTgres -- Biosequence database extensions GObase -- GeneOntology (GO)
extensions PostGraph -- Graph database extensions PostMake -- Data
derivation dependency extensions PostModel -- Model base/data mining
extensions

Each extension implements new datatypes with query operators and other
tools, providing powerful large-scale query and analysis, quick
inclusion of new types of biological information, and integration of
diverse existing bioscience data. For example, two important datatypes
implemented in the modules above are biosequence locations and graphs,
and query operators include BLAST access and graph component extraction.

BioPostgres illustrates how the extensibility of PostgreSQL and
open-source development can be harnessed for bioscience data management.
Modules are added to a user's PostgreSQL source tree as needed; each
module is compiled separately and installed in a loadable library
directory. PostgreSQL itself is \_not\_ recompiled, but instead permits
library modules to be dynamically linked into a database -- added "on
the fly" -- with appropriate SQL commands.

BioPostgres is being developed at the Center for Computational Biology
(CCB) at UCLA. Currently all modules are distributed under the GNU GPL.

Web site: www.biopostgres.org

## GObase

Ruey-Lung Hsiao, UCLA

Friday August 4th, 9:30am

The Gene Ontology (GO) defines standard vocabulary for biological terms
in three aspects -- molecular functions, biological processes, and
cellular components. Its wide acceptance and semantic annotation has led
to a wide range of applications -- semantic integration, functional
analysis, and microarray gene clustering, to name a few. It represents
an important new route for connecting information of different types and
has become an essential component in system biology.

The success of the GO underscores the importance of having ways to
manage, query and visualize it. Despite this importance, most
researchers still use an inefficient way to represent and query the GO.
The central data structure of the standard relational database for the
GO consists of two tables: term and term2term. The term table keeps
track of the basic information, such as accession number and term type,
of a particular GO term and term2term represents the relationship
between two terms (i.e., edges in the term graph). However, most queries
for ontology are recursive in nature (One example: find all the
descendants of a particular node), this representation in conjunction
with SQL can fare poorly under a variety of performance measures.

In order to resolve this issue, the GO database pre-computes the
transitive closure of the graph to keep track of every descendants of
the node in the graph. In this way, graph traversal queries can be
answered through this table without issuing recursive SQL commands.
However, the pre-computation of transitive closure leads to very
inefficient usage of storage space by storing a huge number of node
pairs. There is a clear and significant need for better support of GO
representation.

To address these issues we developed the GObase system, a
publicly-available open-source platform for the management, query, and
visualization of GO information. GObase is a graph database, implemented
as an extension of the PostgreSQL database with a graph datatype. This
datatype permits storage and (with addition of new functions)
sophisticated query of graph data. The graph representation is both more
natural and more efficient for queries than the widely-used GO
relational database. There are existing browsers for visualizing GO
information, but the GO Term Viewer of GObase provides a more powerful
interface, allowing both interactive query and interactive annotation of
GO terms. In addition, GObase also links the GO with various other
biological information resources.

website: www.go-base.org license: GNU General Public License

## BioMoby

Martin Senger, International Rice Research Institute, Philippines

Friday August 4th, 10:00am

The Generation Challenge Programme (GCP) is an international
agricultural research consortium, currently numbering 20 agricultural
research institutes, working on the characterization of plant genetic
resources and the application of comparative genomics, toward crop
improvement for the developing world. Given the global dispersion of GCP
partners, distributed access to informatics resources is a major
challenge. Open source projects, such as BioMoby, are essential for
linking GCP components into a coherent information gateway.

The BioMoby is an integration tool helping to connect databases,
analysis programs, and other resources into a unified distributed
system, linking gene discovery with genetic resource characterization
and crop evaluation data. GCP developers added new components there,
some of them are presented here.

BioMoby Dashboard is a rich standalone Java application for BioMoby
developers, assisting through the whole process of creating, deploying
and using Biomoby services. It has a plug-in architecture allowing
additional extensions.

BioMoby MoSeS ("Moby Service Support") is a set of code generators that
transform information and ontology trees stored in a central service
registry into Java source code, helping developers of new services to
concentrate only on business logic and not on the protocol and messaging
details. Such approach guarantees scalability of the developing process.

BioMoby Environment is an automated way to regularly check if the
deployed services are running and producing correct results. In the
environment with so many participants, such quality control tool is
essential.

BioMoby can cooperate with other integrating tools. A separate project
"BioCASE & BioMoby" shows how to use BioMoby to "wrap a wrapper". The
BioCASE integrates access to many databases, and BioMoby spreads its
data into existing clients and networks.

Links: GCP <http://www.generationcp.org> BioMoby <http://biomoby.org>
BioMoby Java projects:
<http://biomoby.open-bio.org/CVS_CONTENT/moby-live/Java/docs/> BioCASE
<http://www.biocase.org>

## XRATE

Ian Holmes, Ph.D, Berkeley University

Friday August 4th, 11:00am

A big hit in the past couple of years has been the "phylo-HMM", a
multi-sequence HMM employing Felsenstein's pruning algorithm to compute
emission scores. (Stochastic grammar extensions to this idea include
phylo-GHMMs and phylo-SCFGs.) The phylo-HMM idea was first introduced
for genome analysis by Churchill and Felsenstein, and further developed
e.g. for RNA structure prediction by Knudsen and Hein. The use of
phylo-grammars by Siepel, Pedersen, Bejerano, Haussler et al for gene
prediction, evolutionary analysis of rate variation, and other forms of
genome annotation has gotten lots of attention in recent years.

Much of the appeal of phylo-grammars is the straight transfer of
intuition and expertise from the areas of HMMs and SCFGs. However, the
well-known EM algorithms used to train these models (Baum-Welch,
Inside-Outside) are a little less straightforward to apply to phylo-
grammars. In contrast to (say) Baum-Welch, the phylo-EM algorithm is
pretty hairy and not something you'd really want to implement twice.

In the past 4 years we have taken the theory of phylo-EM algorithms from
a theoretical treatment (Holmes & Rubin, JMB, 2002) up to a full- blown
open-source implementation of a general phylo-grammar prototyping,
training and annotation engine (XRATE). Grammars can be specified using
a Scheme-like format, "trained" on alignments using phylo-EM, and then
used to annotate alignments. The phylo-EM code in our open-source C++
library can also be linked to by external applications (e.g. Jakob
Pedersen's EVOFOLD program, which has been used to investigated
recently-evolving human ncRNAs). Several developers have contributed
full-time to the process, and there is considerable stability, including
a battery of automated tests.

XRATE is an easy-to-use Unix app that brings the unrestricted power of
phylo-grammars in reach of a first-year grad student or smart undergrad.
In a historical aside, XRATE has its roots in a grammar compiler,
TELEGRAPH, that was itself based on Ewan Birney's DYNAMITE (and is
related to Guy Slater's EXONERATE). TELEGRAPH was presented at BOSC
2000. At BOSC 2006, I'll show how far XRATE has come by giving a tour of
its rate-measurement and annotation abilities, accompanied by
visualizations of the interesting variety of patterns (covariation,
neighbor-dependence, conservation, lineage-specific acceleration,
selection...) that can be observed in the mutation rates of genomic
features.

## Twease

Matt Wood, Ph. D. Cornell University.

Friday August 4th, 11:30am

With 16 million abstracts available in Medline, most searches match more
documents than is possible to read. We asked if sentence level searches
would be more effective in retrieving articles of interest than the
whole abstract method currently used to support most biomedical
searches. We present and evaluate a web-based tool to search Medline at
the sentence level (available from <http://www.twease.org/>). The tool
indexes each sentence of Medline individually and provides features that
help correct for the lack of context introduced when searching sentences
separately from the rest of the sentences in an abstract. We evaluated
Twease with queries assembled from an independently obtained
protein-protein interaction dataset (2,789 distinct interactions), as a
measure of performance when retrieving abstracts with conjunctive
queries of biomedical interest. Experimental results indicate that, on
average, the first 25 Twease hits contain as many relevant abstracts as
the first 100 PubMed hits. The first 25 Twease hits are also twice more
likely to contain a relevant hit than the first 100 PubMed hits. These
results indicate that sentence level searches, as implemented in Twease,
are a competitive strategy when searching the biomedical literature for
articles about multiple concepts (e.g., protein-protein interactions, or
disease gene/protein relationships). Because a Twease index can be
created directly from a text collection and does not require custom
semantic resources, the approach implemented in Twease can be used to
index and search any text collection of abstracts or full text articles.
Twease implements highly scalable algorithms and approaches that will be
discussed during the presentation and is released under the GNU General
Public License. The distribution can be downloaded from:
<http://icb.med.cornell.edu/crt/twease/index.xml>.

## ZMap

Roy Storey, Sanger Institute, Hinxton, Cambridge

Friday August 4th, 1:30pm

We present a software package, ZMap, that is a visualisation tool for
genomic features. The software is a multi-threaded application written
in C, utilising the gnome toolkit (GTK2) and draws features on the
foocanvas. ZMap accepts input from multiple sources in multiple formats
across multiple genomes and is written in way that the addition of
further formats is made as trivial as possible. Currently the list of
formats includes GFF v2 and DAS1 which may reside in any one of; a file,
an acedb instance, a http server. Multiple genomes and their associated
features can be displayed in a single view as aligned blocks providing
support for comparative annotation.

A wide complement of browser features are implemented in the ZMap GUI.
Users may zoom to any resolution in the range from individual bases to a
whole chromosome. The display may be split in both vertical and
horizontal axis multiple times in a way akin to emacs. The contents of
the display are completely copied in order that, as for emacs, the two
views are independently scrollable. In this way it is possible to
utilise screen space to view both ends of features at a much higher
resolution than would otherwise be possible. Users are able to perform
operations on the full sequence context, such as reverse complement,
print, export and search.

Internally ZMap has a client/server architecture, where the GUI control
thread acts as the client making requests to each server that
communicates with a unique source. Each server runs within its own
thread enabling the graphical thread to remain responsive. Various
servers may add to the display at any point during the lifetime of the
application. The features are merged with the current context allowing
features from multiple sources to be viewed along side each other. As
threads are separated from the control interface a user can kill the
request in the event of an unresponsive or slow server.

ZMap does not natively include any utility for editing the features
which it displays. It does however provide a powerful external interface
with which to modify the features which are displayed on the canvas.
ZMap utilises the X11 atom mechanism for interprocess communication, via
which it is possible to communicate in xml. A perl module X11:XRemote is
provided to facilitate ease of integration with perl annotation tools.
Using this interface Sanger's production annotation tool otterlace is
used to annotate sequence present in the Otter database which in turn
updates to the Vega website.

Software License ----------------

The GNU General Public License (GPL) Version 2

## CaIntegrator

Subha Madhavan, Ph.D. , National Cancer Institute

Saturday August 5th, 10:00am

Progress in finding better therapies for cancer treatment is hampered by
the lack of opportunity to integrate biomedical data from disparate
sources to enable translation of therapies from bench to bedside and
back. Hence, a critical factor in the advancement of biomedical research
and delivery is the ease with which data from clinical trials can be
integrated, redistributed and analyzed both within and across functional
domains. Novel biomedical informatics infrastructure and tools are
essential for developing individualized patient treatment regimens based
on the specific genomic signatures in each patientsed gene expression,
Copy number Abnormality (CNA), SNPs, clinical trials data etc.) in a
cohesive fashion.

Following are some of the high-level features of the caIntegrator
framework:

\- N-Tiered Architecture: The caIntegrator framework is implemented
using Java 2 Enterprise Edition, a Data Warehouse, and various other
open source technologies. It is designed to conform to an n- tiered
architecture that includes several layers: A web-based graphical user
interface, a business object layer, server components that process the
queries and result sets, a data access layer and a data warehouse.

\- A Common set of interfaces (APIs) and a domain object model: The
domain object model called CGOM (Clinical Genomics Object Model)
provides standardized programmatic access to the integrated biomedical
data collected in the caIntegrator data system. The model represents
data from clinical trials, microarray-based gene expression, SNP
genotyping and copy number experiments, and Immunohistochemistry-based
protein assays. Clinical domain objects in CGOM allow access to Clinical
trial protocol, treatment arms, patient information, sample histology,
clinical observations and assessments. Genomic domain objects allow
access to biospecimen information, raw experimental data, in-silico
transformation and analyses performed on the raw experimental datasets
and biomarker findings. The application's user interface communicates
with its caIntegrator-based middle-tier services via domain as well as
business objects.

\- A real-time analytical service that provides on-the-fly computational
analysis capability for caIntegrator applications and currently supports
class comparison analysis, principal component analysis and clustering
analysis. It is designed to easily incorporate other types of analysis
in the future, and scale to provide performance.

\- The caIntegrator data system consists of a star schema database,
which contains the clinical, and annotation data as dimensions,
pre-calculated gene expression copy number data as facts. For
performance reasons, normalized gene expression data used by the real
time analysis module is stored as R-binary files.

\- A plotting interface to allow visualization of genomic data (copy
number scatter plots and ideogram) via the webGenome application
(http://webgenome.nci.nih.gov).

The overall goal of the caIntegrator project is to provide a
caBIG-compatible (https://cabig.nci.nih.gov/guidelines_documentation)
framework with the infrastructural components needed to develop
enterprise level translational applications. One such reference
implementation at NCICB is REMBRANDT (Repository of Molecular BRAin
Neoplasia DaTa) - <http://rembrandt.nci.nih.gov>. REMBRANDT is a
powerful and intuitive informatics system designed to integrate genetic
and clinical information from brain tumor clinical trials for improved
research, disease diagnosis, and treatment. It provides researchers with
the ability to perform ad hoc querying and reporting across multiple
data domains, such as Gene Expression, Chromosomal aberrations and
Clinical data. Scientists are able to answer basic questions related to
a patient or patient population and view the integrated data sets in a
variety of contexts. Tools that link data to other annotations such as
cellular pathways, gene ontology terms and genomic information are
embedded within this system. Two other cancer study applications that
are being developed using the caIntegrator framework are:

\- I-SPY Breast cancer trial: The primary object of the I SPY Trial is
to identify surrogate markers of response to neoadjuvant chemotherapy
that are predictive of pathologic remissions and survival in Stage III
breast cancer. Goal is to identify Molecular markers and/or MRI results
that predict 3-year disease-free survival in these patients.

\- CGEMS: Cancer Genetic Markers of Susceptibility (CGEMS) is an NCI
project to identify genetic alterations that make people susceptible to
prostate and breast cancers. Goal of CGEMS is to analyze the entire
genome for most common type of SNPs that are associated with each of
these diseases.

caIntegrator knowledge framework offers a paradigm for rapid sharing of
information and accelerates the process of analyzing results from
various biomedical studies with the ultimate goal to rapidly change
routine patient care.

Resources:

CaIntegrator website: <http://caintegrator.nci.nih.gov> REMBRANDT
(caIntegrator reference implementation): <http://rembrandt.nci.nih.gov>
REMBRANDT application URL: <http://rembrandt-db.nci.nih.gov>
CaIntegrator open source license:
<http://ncicb.nci.nih.gov/download/caintegratorlicenseagreement.jsp>

## SHOGUN

Soren Sonnenburg, Fraunhofer Institut, Max Planck Society.

Saturday August 5th, 11:00am

We have developed a Machine Learning toolbox, called SHOGUN, which is
designed for large scale sequence analysis tasks appearing in
computational biology. It features a number of machine learning
algorithms such as Support Vector Machines \[3\] for classification and
regression, but also Hidden Markov Models, Multiple Kernel Learning \[1,
8\], Linear Discriminant Analysis, Linear Programming Machines and
Perceptrons. Most of these algorithms are able to deal with several
different data types including sparse vectors and sequences.

SHOGUN provides a generic SVM object interfacing to seven different SVM
implementations, among them are LibSVM\[2\] and SVMlight\[5\], two
state-of-the-art SVM implementations. Each of these can be combined with
a variety of kernels. The toolbox not only provides efficient
implementations of the most common kernels, like the linear, polynomial,
Gaussian and sigmoid kernel, but also comes with a number of recently
proposed string kernels including the Fischer & TOP kernel \[4, 15\],
the Spectrum kernel \[6\], the locality improved kernel \[16\] and the
weighted dregree kernel \[7, 13\]. For most of the sequence kernels we
have implemented optimized data structures such as tries to speed-up
training and evaluation of SVMs.

We have successfully used this toolbox to tackle the following sequence
analysis problems: Protein Super Family classification\[15\], Splice
Site Prediction\[10, 11\], Interpreting the SVM Classifier \[12, 8\],
Splice Form Prediction\[7\], Alternative Splicing\[9\] and Promotor
Prediction\[ 14\]. Some of them come with no less than 10 million
training examples, others with 7 billion test examples.

SHOGUN is implemented in C++ and interfaces to MatlabTM, R, Octave and
Python/Numarray. The Source Code is freely available at
<http://www.fml.mpg.de/raetsch/projects/shogun> under the GNU General
Public License, Version 2.

References F. R. Bach, G. R. G. Lanckriet, and M. I. Jordan. Multiple
kernel learning, conic duality, and the SMO algorithm. In C. E. Brodley,
editor, Twenty-first international conference on Machine learning. ACM,
2004. C.-C. Chang and C.-J. Lin. Libsvm: Introduction and benchmarks.
Technical report, Department of Computer Science and Information
Engineering, National Taiwan University, Taipei, 2000.

## XMLPipeDB

Kam Dahlquist, Department of Biology, Loyola Marymount University

Saturday August 5th, 11:30am

XMLPipeDB is an open source suite of Java-based tools for automatically
building relational databases from an XML schema (XSD). XMLPipeDB
provides functionality for managing, querying, importing, and exporting
information to and from XML data with minimum manual processing of the
data. While its applicability is fairly general, the original motivation
for XMLPipeDB was to create a solution for the management of biological
data from different sources that are used to create Gene Databases for
GenMAPP (Gene Map Annotator and Pathway Profiler), software for viewing
and analyzing DNA microarray and other genomic and proteomic data on
biological pathways. The creation of Gene Databases for GenMAPP has been
difficult because there are a number of different gene ID systems in
common usage, necessitating that we relate one set of gene identifiers
to the other. Currently, the GenMAPP Gene Databases use the integrated
data source from Ensembl for this task. However, this limits the number
of species that can be represented in GenMAPP to the mostly animal
species supported by Ensembl. Here we report that we have used the
XMLPipeDB software tool chain to create relational databases for UniProt
and Gene Ontology. In turn, we have used these databases to generate
UniProtcentric GenMAPP Gene Databases for Escherichia coli and other
bacterial species, extending the functionality of GenMAPP to species not
currently supported by the GenMAPP.org project team. Moreover, since
XMLPipeDB can create the relational databases based solely on the XSD
and XML files, it will be more robust to changes in the source files
made by the data providers.

XMLPipeDB has the following tools for developers and database designers:
the XSD-to-DB application takes a well-formed XSD or DTD file and
converts it into a collection of Java source code and Hibernate mapping
files that allows XML files based on that definition file to be read
into a relational database. XSD-to-sses that provide functions needed by
many XMLPipeDB database applications. Specifically, the library includes
reusable classes for: importing XML files into Java objects, saving
these XML-derived Java objects to a relational database, querying the
relational database using either HQL (Hibernate Query Language) or SQL,
and configuring a client application to communicate with a relational
database. Finally, GenMAPP Builder is an application for creating the
GenMAPP Gene Database files.

GenMAPP Builder has been tested for use with the open source PostgreSQL
relational database, but can be used with any other relational database
management system for which a JDBC driver is available. JDBC-to-ODBC
connectivity is used to transfer data from this relational database to a
Microsoft Access MDB file, which is the format expected by the GenMAPP
application.

XMLPipeDB was developed by graduate students as part of a team-taught
course in bioinformatics that was then extended into a second workshop
course on open source software development. The primary objectives of
this course are to gain real world experience with open source software
development, learning key open source development concepts, gaining
proficiency with tools that are frequently used in the open source
community (many of which are used in effective software development in
general), and making a concrete contribution to an open source software
project. XMLPipeDB is available under the GNU Library or Lesser General
Public License (LGPL) at <http://sourceforge.net/projects/xmlpipedb>.

## BioRuby

Toshiaki Katayama, Human Genome Center, Institute of Medical Science,
University of Tokyo (Part 1)

Pjotr Prins, Wageningen University (Part 2)

Saturday August 5th, 1:30pm

Part 1: BioRuby 1.0 and the BioRuby shell

As one of the Open Bio\* projects hosted by Open Bio Foundation, we have
been developing the BioRuby, a Ruby library for bioinformatics. In this
February, we have released the BioRuby version 1.0 coming with various
new features, bug fixes, unit tests and documentations. In this talk, I
will describe what we have achived with the 1.0 release and our future
plans.

The Open Bio\* libraries have been successful as toolkits to develop
customized bioinformatics pipelines, however, it was still difficult for
the biologist to utilize the libraries as their daily tool. There can be
two main reasons, (1) larning a programming language is a burden for
their spare time and (2) there are \*too\* many ways to do it! Thus, we
included the BioRuby shell, a newly developed CUI (command line user
interface) for the BioRuby library. BioRuby shell integrates and
abstracts various ways of entry retrieval, flatfile processing, and
accessing of web services, even with enabling users to utilize all
functionality of Ruby and BioRuby without writing any script file. In
the shell, objects and the history are conserved across the sessions,
and a script to reproduce the procedure can be automatically generated.

Other enhancements in BioRuby 1.0 include unit tests and documentations.
Hohman started to add unit tests for some essential classes in BioRuby
and Nakao has completed \>1000 tests to make our library stable. We also
added a English guideline to contribute our projects, and thanks to it,
several developers joined to our project. Aerts and Raaum have been
worked on the documentation format specification (RDoc format) and
adding detailed API documentations. Goto translated Japanese tutorial
and Prins improved the English version. Wennblom launched
<http://bioruby-doc.org/> site to develop further BioRuby
documentations.

Part 2:

With the world wide Ruby user base growing (in part thanks to Ruby on
Rails) we are putting an effort in to increase the adoption of Ruby in
bio-informatics by both improving the documentation of the BioRuby
project and dedicating a significant section to Bio-informatics on the
SciRuby project: a portal for all things scientific and Ruby. The latter
an initiative of the Pragmatic Bookshelf team - which is planned to lead
to a book on Ruby in science (see <http://sciruby.codeforpeople.com/>).

In this talk we present two open source initiatives namely TaxonSearch -
a BLAST post- processor for the genomic mining of taxonomic information
and Ruby Queue (rq), a free and straightforward clustering job
management tool. TaxonSearch stores full taxonomic information of all
matches of a large scale BLAST exercise and allows for complex regular
expression based queries by end users. We used it, for example, to find
putative lateral gene transfer candidates from bacteria to nematodes
(BLASTing EST databases against the NCBI non-redundant database). The
program features a split search and query procedure because the BLAST
search can take a lot of (cluster) time. Once the database has been
built, queries can happen on a simple user workstation with no other
dependencies beside the Ruby interpreter.

Ruby Queue (rq) can be used to drastically reduce the overhead and
complexity of distributing work to a collection of commodity
workstations. Ruby Queue does not depend on other clustering tools and
can be run on a number of Linux machines mounting a shared network file
system (NFS).

Both TaxonSearch and Ruby Queue tools are also relevant to non-Ruby
users. As a conclusion we will try to clarify why we think Ruby as a
language is to play a major role in bio-informatics. TaxonSearch will be
published for BOSC 2006 through both BioRuby and SciRuby projects under
the GPL.

BioRuby code is Ruby licensed (GPL, IIRC) Ruby Queue (rq) is Ruby
licensed (GPL, IIRC) The bio-informatics sections in SciRuby are
published under a creative commons license. Pjotr Prins (see
<http://thebird.nl/>) is a researcher at the Department of Nematology,
Wageningen University and a visiting research fellow at the Department
of Bio-informatics at the University of Groningen.

Pjotr initiated the OSS Cfruby, xParrot and GenEst projects and
contributes to BioRuby and SciRuby.

Ara Howard (see <http://sciruby.codeforpeople.com/>) is a professional
research assis- tant at the National Geophysical Data Centre (NGDC).

## NESCent

Hilmar Lapp, Todd Vision, National Evolutionary Synthesis Center
(NESCent), Durham, NC

Saturday August 5th, 1:30pm

The National Evolutionary Synthesis Center (NESCent) was founded in
November 2004 with funding from the U.S. National Science Foundation
with the goal of addressing "grand challenge" questions in evolutionary
biology. NESCent pursues this goal by sponsoring synthetic science that
is highly collaborative, involving teams of researchers from
institutions around the globe, and also highly interdisciplinary,
reaching across disciplines such as genetics, developmental biology,
systematics, ecology, geography, and paleontology. Much of this research
is also informatics-intensive, utilizing and combining datasets,
annotation, and analysis methods from multiple domains.

NESCent is well positioned to play a leading role in improving the
infrastructure for synthetic science in evolutionary biology. Areas of
critical need include data and metadata sharing standards and
technologies, open libraries to support standard data exchange formats,
software interoperability and usability, and training a critical mass of
open source software developers within the discipline.

We describe three collaborative informatics projects at NESCent that are
helping to enable synthetic science in different ways. First, we are
extending GMOD tools and data models to accommodate a key evolutionary
datatype, population variation. Second, we are establishing a searchable
meta-data registry for evolutionary data to promote data reusability.
Third, we are helping systematists and developmental geneticists connect
knowledge about zebrafish mutants, on the one hand, and natural
phenotypic diversity among related fish in the Order Cypriniformes, on
the other, through semantic mediation.

Finally, we encourage participation and seek input from the informatics
community at large. We are sponsoring 'hackathons' and software-oriented
working groups for the development of open software libraries in
evolutionary biology. We are also soliciting whitepapers to identify
areas of focus for the future (see <http://www.nescent.org/>). NESCent
is committed to open-source development and to partnering with existing
open-source projects wherever possible.
