---
layout: default
title: Welcome
nav_order: 1
description: "Home"
permalink: /
---

# Penn Brain Science Center cluster computing resources

This is the index page for the [Penn Brain Science
Center](https://pennbrain.upenn.edu) cluster computing documentation. 

The BSC computing cluster is hosted by DART (formerly PMACS) in their "Limited
Performance Computing" (LPC) environment. 

The LPC is distinct from the PMACS [High Performance Computing](https://www.med.upenn.edu/hpc/) (HPC) service. The
HPC is better suited for large-scale data processing beyond the capabilities of
the LPC. 

The LPC serves multiple different labs and centers. Some groups affiliated
with the BSC also have independent LPC resources outside of the BSC cluster,
which are generally similar, but not identical to the BSC. Therefor the LPC
documentation provided by other LPC users can be a useful source of information
to BSC users, but some details may differ.


1. TOC 
{:toc}

# LPC overview

The LPC is a shared resource for cluster computing, supported by DART and the
BSC. The LPC provides a substantial upgrade in hardware and software performance
compared to the previous CFN cluster. Like the old CFN cluster, the LPC is a
Linux computing environment with multiple compute nodes, a grid engine job
scheduler, and backed-up network storage. 

Brain Science Center (BSC) Computing Cluster. The BSC manages a dedicated neuroimaging computing cluster with 9 compute nodes. There are 8 PowerEdge R640 Servers each with 2 Intel Xeon Gold 6240R 2.4G processors that have 24 cores, 384GB of RAM, and and 8GB RAM per core along with 2TB of SSD local

storage for scratch space, 10Gig Dual Ethernet ports, and 1Gig Quad Ethernet ports. In addition there is 1 Dell PowerEdge 640 high memory node with 2 Intel Xeon Gold 6240R 2.4G processors that have 24 cores each with 768GB of RAM and 16GB RAM per core, 2TB of SSD local storage for scratch space, 10Gig Dual Ethernet ports, and 1Gig Quad Ethernet port, All nine nodes are housed in the Perlman School of Medicine’s commercial-grade server room with redundant power supplies; UPS power backup systems; fire suppression system; and 24-hour restricted access and security. The BSC cluster is connected to the PMAC local “cloud” storage array that provides economical storage with backup and archiving capabilities

## Access

Please see the article on [accessing the PMACS cluster](/docs/clusterEnvironment/access.md) about how to access the BSC PMACS cluster.

## Security and privacy

All data on the cluster should be de-identified. Contact PMACS if you have
specific requirements

## Software

## User groups

## Billing

## Additional PMACS resources


## LPC accounts

How to get an LPC account.

## LPC vs CFN cluster usage

Main article: [LSF for CFN users](/docs/clusterEnvironment/cfnToLPC.md)

The LPC cluster uses the IBM LSF system for parallel computing, while the CFN
cluster used the Sun Grid Engine. While many of the same concepts apply, there
are several differences in how jobs are submitted and run. 

## LPC Access

BSC LPC [Access](/docs/clusterEnvironment/access.md)

# External resources


## PMACS documentation (requires Pennkey authentication)

[LSF Basics](https://wiki.pmacs.upenn.edu/public/LSF_Basics) 


## IBM LSF documentation

[Full LSF
documentation](https://www.ibm.com/support/knowledgecenter/en/SSWRJV_10.1.0/lsf_welcome/lsf_welcome.html)


## Computing skills

Using the cluster effectively requires familiarity with the Linux command line
and basic scripting. There are many resources online for this. Penn personnel
can access LinkedIn Learning (formerly Lynda), by signing in with their PennKey at

http://linkedinlearning.upenn.edu/


### Linux and shell scripting

Some courses of interest:

[Learning Linux Command
Line](https://www.linkedin.com/learning/learning-linux-command-line-2) this
course gives an introduction to using the Linux command line.

[Learning Linux Shell
Scripting](https://www.linkedin.com/learning/learning-linux-shell-scripting-2018)
this course covers basic shell scripting.

[Linux: Bash Shell and
Scripts](https://www.linkedin.com/learning/linux-bash-shell-and-scripts) this is
a longer course on shell scripting that covers the basics but also gets into
more advanced topics. Shell scripting is powerful and convenient to run basic
tasks quickly, but users should consider another language such as Python for
complex systems. 
