---
title: SolutionChallenge
permalink: SolutionChallenge
layout: wiki
---

Back to [BOSC 2010](BOSC_2010 "wikilink")

## OpenBio solution challenge: Project updates at BOSC 2010

One of the traditional items we've had at the conference is project
updates from open source bioinformatics libraries, like BioPerl,
BioJava, Biopython, BioRuby and EMBOSS. This year, we're planning to
organize these talks around a central theme: the OpenBio solution
challenge. We start with a biological question of general interest, and
project talks focus around how you would solve that problem using your
toolkit and programming language.

This is meant to provide a challenge for OpenBio contributors, a nice
tutorial style overview of various projects and approaches for other
programmers, and a fun opportunity to compete and learn from other
projects. Conference attendees will vote on their favorite solution,
with the winner receiving fame and fortune (warning: fortune not
guaranteed).

The challenge is open to any interested participants. Please submit an
abstract for BOSC with information about your project and that you are
interested in participating in the solution challenge session. Introduce
yourself and your ideas on the Open Bio mailing list as well.

## Guidelines

- The goal is to pick a challenging problem that demonstrates the
  utility of a bioinformatics approach to answering the question, not
  necessarily an unsolved problem like the [Netflix
  Prize](http://www.netflixprize.com/).

<!-- -->

- Feel free to use any publicly available programs and libraries in
  solving the problem. If you are solving a problem in Python, we
  certainly want to see how the language and toolkits help you do that
  most efficiently, but re-writing BLAST in Python makes no sense. How
  you integrate the external programs into your automated analysis
  pipeline is of extreme interest.

<!-- -->

- We can select from one overall challenge or a panel of challenges.
  We'd like to provide some overlap to help compare and contrast various
  approaches, but some challenges may fit better with a focus of a
  toolkit then others.

<!-- -->

- The winner will be selected by conference participants; everyone who
  sees your talk gets a vote. The criteria conference attendees should
  vote on are
  - Execution of the analysis. How easy is it to understand and
    replicate?
  - Quality of the answer. What interesting biological was discovered?
  - Uniqueness of the approach. What elements of the toolkit make it
    useful for the problem?

## Project ideas

These are collected project ideas from various members. Please create a
wiki account for yourself and add your own ideas. As a group we will
decide on one or more challenges to use:

- Fly RNA-seq gender analysis. Start with short read alignments in [SAM
  format](http://samtools.sourceforge.net/SAM1.pdf) from the [modENCODE
  project](http://intermine.modencode.org/release-16/experiment.do?experiment=RNA-seq%20support%20of%20the%20ChIP%20data).
  Alignments of total RNA from both male and female flies are available.
  Your goal is to use these alignments to highlight major expression
  differences between the genders. This will involve organizing
  alignment locations relative to genomic features, identifying
  differences, and providing summary charts and tables that explain the
  most interesting results.

## Discussion

Your thoughts and project ideas are very welcome. Please use the open
bio mailing list as a central point of discussion:
<open-bio-l@lists.open-bio.org>