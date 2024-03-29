---
title: 2009 hardware purchase proposal
permalink: 2009_hardware_purchase_proposal
layout: wiki
---

# Proposal to purchase new machines for OBF

## Justification for total replacement of existing servers

**Total Server Refresh - Move to 100% hypervisor-based virtualization**

- Existing servers date back to 2004 and are based on 32bit Pentium 4
  chipsets
- Existing servers running CentOS 4.8, current CentOS is at version 5.4
- No spare server capacity for new service and server requests from OBF
  community
- Only two people (Chris D and Jason S) have 100% full remote control
  including remote-power reboot ability
  - Can not easily/securely provide full remote control to other
    volunteers with existing infrastructure
- We need to move to 64 bits, x86_64 and take advantage of CPU level
  support for virtulization
- Virtualizing our servers and services greatly reduces operational
  burden, makes our IT infrastructure more "portable" should future
  situations demand it and also solves much of our existing issues with
  granting high levels of remote admin access (including console &
  remote power control) to members of our sysadmin team
- New 64-bit hardware with CPU level virtualization support would allow
  OBF to:
  - Run many more servers and services as needed
  - Provide higher levels of performance
  - Provide higher levels of redundancy, safety and portability
  - Allow much greater distribution of administrative powers
  - Consume less datacenter space
  - Consume less datacenter electricity

## Justification for new Email Scanning Appliance

**New Purchase - Mail scanning appliance**

This proposal is to solve a problem that has long been somewhat
invisible to the OBF community - the **extremely** large amount of work
required to handle the massive volume of email traffic that our lists
receive, particularly in dealing with and moderating emails that are
clearly spam but have gotten through our own anti-spam and anti-virus
filters. These messages end up in the moderator queues of all our
mailing lists (dozens per day, per email list) and represent the single
largest operational and administrative burden for OBF volunteers.

The fact is that in 2009 the free and open source methods for anti-spam
and anti-virus can not keep up with the current methods used by the bad
guys. The most common source of spam these days are compromised PC
systems that send email in small volumes, via seemingly legit accounts
and at rotating intervals. The PC-based botnets are much harder to block
via greylisting and blocklists than the previous generation of spammers
who preferred sending large volumes of email through a smaller
collection of hosts.

**Current OBF methods of anti-spam and anti-virus include**:

- Greylisting in effect on all inbound email from unknown senders
- All inbound/outbound email scanned by clamAV for viral payloads
- Email that passes the clamAV test gets routed through MIMEDefang for
  additional scrutiny
- Email that passes clamAV and MIMEDefang gets processed by SpamAssassin
- A high SA score causes the email to be discarded automatically

Even with the above methods in place, a huge amount of spam still gets
through and clogs up the moderator queues of our very active mailing
lists.

**Bad effects of the spam deluge:**

- Overworked volunteer list administrators
- Legit emails being lost or deleted in bulk moderator cleanup attempts
- Once open mailing lists have had to become more closed and harder to
  reach
- Overall our mailing list community is not as open/accessible as it has
  been in the past, due to the anti-spam defenses we've had to emplace
- Our community is not as open as it could or should be

**Commercial Solutions Exist**

For 4 years, BioTeam Inc. (the company that donates datacenter space to
OBF) has been routing it's own corporate email through a
hosted/outsourced email cleaning service operated by MailFoundry Inc.
(http://www.mailfoundry.com). The hosted service charges a flat monthly
fee per email address protected. Over the years Bioteam has consistently
seen upwards of 90% of total email volume being spam, malware-laden or
otherwise unwanted. Via MailFoundry scanning, the 90% of "bad" email is
caught and isolated before hitting the mailserver. False positives do
exist but experience shows that they occur on the order of 3-4 times per
year.

However, the hosted or outsourced services offered by MailFoundry and
competitors like Postini, Google etc. will not work for the OBF because
they typically charge fees based on **per-email** and **per-domain**.
Given that we run dozens of mailing lists via dozens of domains and that
each mailing list has 6-7 related addresses ("-admin, "-help", etc.) our
research has shown that we can't really make use of a hosted solution
that charges by domain or email address in any financially reasonable
way.

Our recommended solution is to spend real money on a hardware email
scanning appliance from www.mailfoundry.com. For the cost of the
appliance and the annual update fees we gain the ability to protect an
**unlimited number of email addresses and domains**. This alone will be
a huge win for the OBF and if it works really well we may be able to
open our lists to ad-hoc messages from the general public again. This
also could allow us to offer more individual email services to OBF
projects and volunteers.

The commercial solution is expected to cost \$1,200 - \$1,400 USD
depending on support options selected.

## Proposed purchases

Proposals exist to purchase two main infrastructure devices:

- A pair of quad-core Intel Nehalem server systems with 24GB RAM &
  remote management capability (including KVM) all packaged into a
  single "1U twin server" space and power-efficient package. For an
  example of this type of system see this URL
  <http://www.siliconmechanics.com/c1159/1u-twin-servers.php>
- A dedicated email scanning appliance from <http://mailfoundry.com/>

**Server Quotes**

- \$5000
  ![](Silicon_Mechanics_Quote_173894.pdf "Silicon_Mechanics_Quote_173894.pdf")
- \$1400 MailFoundry 1150 Email Filtering Appliance

### In-kind Donations

It is not 100% set yet, but it is highly likely that BioTeam Inc. will
be able to donate a 16-disk SATA storage server to the OBF for use as a
NFS fileshare among the virtualization platforms. When used with Citrix
XenSever or VMWare this NFS storage pool will allow for live migration
of running servers between physical virtualization hosts. This will
allow for hardware failures and maintenance to have minimal or no impact
on OBF operations.

## Deployment and upgrade plan

- Decomission old machines, helps free up **donated** rackspace from
  BioTeam
- Setting up worldwide mirrors for backup purposes (rsync scripts from
  the repository?)
  - Our 2 most valuable components are src code and mailing list
    (archives and membership). Losing these or being down is a HUGE
    problem. Can we insure these are protected and redundantly
    preserved?
- How can we balancing security, all volunteer sysadmin team, moderate
  latency in response to issues (due to all volunteer nature)

# Community requests

- Latest and greatest src code tools - GIT/Mercurial, previously Trac
  was also requested.
  - Has been problematic to support because we currently don't allow
    HTTP access to dev machine
  - Can we setup NFS + httpd on separate machine with mirrored FS
    (read-only) or NFS(read-write) or other system?
- How do we keep Wiki's up-to-date w software - better wikifarm support?
