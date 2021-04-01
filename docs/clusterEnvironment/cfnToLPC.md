---
layout: default
title: LPC basics for CFN users
parent: Cluster Environment
has_toc: true
---

# LSF user guide for CFN (chead) users
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# LSF vs SGE

The CFN cluster used an implementation of the (deprecated) Sun Grid Engine
(SGE). The LPC uses IBM's Load Sharing Facility (LSF) system.

There is a general guide to the LSF for SGE users here: [SGE to LSF
Conversion](https://www.med.upenn.edu/hpc/sge-to-lsf-conversion.html).


## CFN cluster specifics

| SGE | LSF | Notes |
+-----+-----+-------+
| qstat | bqueues | List available queues |
| qrun | bsub | Submit jobs |
| qstat | bjobinfo | get job info |


## Generic job submission script


# General cluster organizational differences

The grid computing system 
