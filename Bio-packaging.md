---
title: Bio-packaging
permalink: Bio-packaging
layout: wiki
---

If you are in any way interested in software packaging and deployment
for bioinformatics you can meet like-minded people on the Open
Bioinformatics Foundation (OBF) [bio-packaging mailing
list](http://lists.open-bio.org/mailman/listinfo/bio-packaging).

On the mailing list we discuss issues around packaging and deploying
software: anything that concerns dependencies, multiple version support
and/or reproducibility. The general idea is to come up with solutions we
can share across environments and construct (shared) pipelines out of
them.

## Generic packaging systems

### GNU Guix

[GNU guix](https://www.gnu.org/software/guix) is a package manager for
the Gnu/Linux operating system. Bioinformatics packages are constructed
[here](http://git.savannah.gnu.org/cgit/guix.git/tree/gnu/packages/bioinformatics.scm).
GNU Guix can be run inside any Linux distribution (it is distribution
agnostic because all software installs under /gnu). There may be
OSX/Cygwin support in the future, but currently the targets are Linux
and Hurd.

### GNU Guix for bioinformatics

For Bio-packaging we created a [GNU Guix edition for
bioinformatics](https://github.com/genenetwork/guix/wiki/GNU-Guix-for-bioinformatics).
See also GNU Guix
[documentation](https://www.gnu.org/software/guix/manual/guix.html) and
Pjotr Prins' [guix-notes](https://github.com/pjotrp/guix-notes) and
Malcolm Cook's [manual](https://github.com/malcook/sce)

## Language based packaging systems

### Ruby biogems

- [biogems](http://biogems.info/) are Ruby packages (gems) that can
  install globally or in HOME. To make sure gems do not conflict with
  multiple Ruby versions it is possible to use RVM, rbenv and/or GNU
  Guix.

### Python packages

### Perl CPAN

### R CRAN

- <http://cran.r-project.org/>

### Javascript

- node.js npm: <https://www.npmjs.com>
- javascript, bower: <http://bower.io>

## Linux distributions and VMs

### Debian Med

[Debian Med](https://www.debian.org/devel/debian-med/) contains a wide
range of bioinformatics software packages target at Debian Linux and
derivatives. See also the [Debian reproducible
builds](https://wiki.debian.org/ReproducibleBuilds) initiative.

### CloudBiolinux

[CloudBioLinux](http://cloudbiolinux.org) offers genome analysis
resources for cloud computing platforms such as Amazon EC2. The source
code can be found [here](https://github.com/chapmanb/cloudbiolinux).
CloudBiolinux uses a combination of Debian/Ubuntu packages with
linuxbrew and self-compiled software.

### Galaxy

### Docker
