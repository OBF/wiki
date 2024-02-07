---
title: BOSC/liveCD
permalink: BOSC/liveCD
layout: wiki
---

<figure>
<img src="Pear.png" title="The Bosc Pair" />
<figcaption>The Bosc Pair</figcaption>
</figure>

# BOSC Software Distribution

This page is a summary of the discussion at the Bioinformatics Open
Source Conference (BOSC) in Vienna on the 19th July 2007. The focus is
the possibility of an 'enriched' software distribution, curated to add
extra value and built into a Debian based LiveCD.

Debian's package management and procedures guarantee primarily technical
reliability - they ensure that the software will install (so it has
dependencies defined etc) and run successfully on a given architecture.
They do not, however, guarantee that the software is

- used for the right set of problems
- employed in concert with the best suite of complementary tools

work at its full potential and be fully understood by the user. The
'enrichment' is therefore in terms of a set of added content and
metadata for each application that is provided.

Making this available as a LiveCD allows for very quick evaluation of
tools. It may particularly appeal to (self-trained?) bioinformaticians
working in wet-lab environments. Another major concern is its
applicability for the use in training courses - today's students are
tomorrow's scientists. Please send in requests for further adaptations.

## What we add

- All applications must be categorized
  - Who is the software for?
  - Which domains does it address?
  - What pre-requisites are required (in terms of expertise rather than
    other software, for example we can assume that BioRuby is only going
    to be useful if you can first use the base Ruby language)
- All applications have tutorial material, comprising
  - usage scenarios
  - example inputs, data files
  - screen capture video of the tutorial examples
- Meta-level entry to realm of software solutions:
  - Expert endorsement, Find a 'foo-omics' expert and get her to pick
    the set of tools she uses most commonly
    - Make sure we include them!
    - Make this grouping available somehow and use it as a 'here's how
      you get started doing foo-omics'
  - Have an umbrella tutorial linking to each tool tutorial
  - Possibly by creating specific 'foo-omics' user with pre-set
    application menus configured?

### Example applications

- Basic command line tools: emboss, fasta, blast
- Sequence-level protein domain finders: mafft, t-coffee, hmmer
- PDB viewer (preferably one without the MOTIF-1980 look)

### Example data

- Full GenBank file for a bacteria (like E. Coli), FASTA of proteins and
  nuclear types of genetic elements

<!-- -->

- SwissProt (in which format?) - discussion: is quite large, in
  particular text and xml format (1.1GB and 2.1 GB), but FASTA is 121M,
  a constraint to a few core organisms may be appropriate (fully
  sequenced mammals, some pathogens (HIV (ignoring the many variants),
  EBV, Hepatitis B (tiny), Salmonella, Yeast, Plasmodium))

<!-- -->

- Some protein domain database ((some subset of) PFAM preferred, PROSITE
  because of its intuitive regular expressions)

<!-- -->

- Some nice PDB files for viewing structure in flashing 3d (JMol and
  friends)

Preferably we should have the same example represented in different
forms and shapes.

The LiveCD is probably limited by the size of a DVD.

## Aggregate Configuration

If we bundle all the tools certain configuration issues (i.e. tool X
needing to know where tool Y is installed) can be solved before the user
hits them. This implies we can identify useful sets of applications but
see the 'expert endorsement' bit above.

## Book

[Dead tree technology](wikipedia:Dead_tree_edition "wikilink") is still
in favour.

Self publishing websites such as [lulu.com](http://www.lulu.com) can
turn a PDF into a book and publish on demand - no up front cost to us!
We would have to do all the typesetting though.

Distributing printed copy of the tutorials + the live CD or DVD would be
fantastic for training, basically a bioinformatics mres module or three
in a box. In particular one can make sure that what is said in the book
is true with the software on the CD, using the same versions, and
without the student facing installing issues before they know what the
software does.

## Link to Debian

- The Debian community has invested considerable effort already in
  providing packages for Bioinformatics and Scientific Computing in
  general:
  - [Debian-Med](http://www.debian.org/devel/debian-med/)
    ([wiki](http://wiki.debian.org/DebianMed),
    [portal](http://debian-med.alioth.debian.org))
  - [Quantian](http://dirk.eddelbuettel.com/quantian.html)

Strong communication between "upstream" BOSC developers and package
maintainer expected. Packages that are provided in addition through this
BOSC initiative are hoped to find their way into the Debian main
distribution. (package needs to comply with [Debian Free Software
Guidelines](http://www.debian.org/social_contract#guidelines) and
[Debian Policy](http://www.debian.org/doc/debian-policy/) for that)

- overcoming communication barriers with people from the other
  (biology/computational) sides

## Who?

- Steffen Möller \<moeller debian.org\> volunteers as a link to the
  Debian community and to help with expertise in packaging
- Kazuharu Arakawa offers their work on a Knoppix (also Debian)-based
  Bioinformatics CD that is accompanied by a Japanese book (Knoppix for
  Bio Project: <http://knob.sourceforge.jp>) and
  <http://ez-tune-livecd.sourceforge.jp/pukiwiki/> (Live CD creator)
- Darin London \<dlondon ebi.ac.uk\>
- Tom Oinn \<tmo ebi.ac.uk\>
- Stian Soiland \<ssoiland cs.man.ac.uk\>
- Bastien Chevreux \<bach chevreux.org\>

## Getting it started

### Packages

Seed of 10 packages.

Available (see Debian-Med initiative):

- BioPerl
- BioJava
- BioPython
- EMBOSS
- Alignment tools (ClustalW, T-Coffee, Muscle, MAFFT, proda et al.)
- HMMer
- Exonerate, Wise
- RNA tools (RNAhybrid, Infernal)
- Structures (AutoDock, Gromacs, apbs, pymol et al.)

Aiming at:

- [Taverna](http://tarverna.sf.net)
- [BioMart](http://www.biomart.org)

which are all a bit more difficult because of Java library versioning
which is not yet established.

### Tutorials / Book chapters offered:

- Using computational grid with BioPerl and T-Coffee to distribute
  computational load in pattern detection. (Steffen)

### Missing:

- Suiteable subset of databases
- Fancy graphics for desktop and startup screen
- Tutorials
- Pattern describing tools besides HMMER (MEME, spexs, ...?)

To get this started we plan to pick (somewhere around) ten packages
drawn from the assorted participants at BOSC this year.

- Tom actively invites
- Tom passively awaits requests for participation from Developers
- Expecting to extend ez-tune-livecd

## Related work

- [Bio-Linux](http://nebc.nox.ac.uk/biolinux.html) - by the
  [NERC](http://www.nerc.ac.uk) Environmental Bioinformatics Centre
  ([NEBC](http://nebc.nox.ac.uk/))
- [BioLinux](http://www.biolinux.org/)
- [Debian-Med](http://www.debian.org/devel/debian-med/)
- Egon Willighagen's ChemBio
  [LiveCD](http://chem-bla-ics.blogspot.com/2006/05/live-life-sciences-cd.html)
- [Knoppix for Bio Project](http://knob.sourceforge.jp)
- [BioPuppy - Minimal Open Source Linux OS for
  BioInformatics](http://biopuppy.org)