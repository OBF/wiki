---
title: SVN-Developers
permalink: SVN-Developers
layout: wiki
---

# SVN repository access for developers

This page is for open-bio affiliated developers who are making use of
SVN based version control systems rather than the traditional CVS based
systems.

## Access methods

### svnserve operates in tunnel mode only

For security and access control reasons we are not running a daemonized
svnserver process or allowing access via HTTP through the Apache
mod_DAV/svn module methods. The SVN access method that fits best with
our current developer and security model is to run svnserver in "tunnel"
mode on a per-user basis. This means developers will connect and
authenticate via encrypted SSH sessions before svnserver is invoked. In
this scenario svnserver is launched in tunnel mode and runs <em>as the
user who invoked it</em>.

The SVN client protocol makes <b>multiple</b> connections to the
svnserver binary. Since we only allow access via SSH this means you may
be prompted for you developer password <b>several times</b> during some
SVN actions, including `update`, `diff` (over revisions), and `merge`.
The easiest way to circumvent having to enter your password multiple
times is to set up your ssh-agent process or make use of SSH keypairs
for passwordless access via public key encryption. For assistance in
setting this up, email the OBF Helpdesk at <em>support at
open-bio.org</em>.

### Public SVN Access

Partially implemented at this time, we now have a web based SVN viewer
installed:

<http://code.open-bio.org/svnweb/>

Methods for anonymously checking out SVN repositories are still being
worked on. It is highly likely, in fact, that when we deploy public SVN
access it will be via <http://code.open-bio.org>.

## Hosted repositories

### blipkit

Blipkit developer access is achieved only via an SSH tunnel:

    svn checkout svn+ssh://dev.open-bio.org/home/svn-repositories/blipkit/trunk blipkit

## Additional SVN documentation

[Version Control with
SVN](http://svnbook.red-bean.com/en/1.1/index.html)
