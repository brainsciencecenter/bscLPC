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
|-----|-----|-------|
| qstat | bqueues | List available queues |
| qrun | bsub | Submit jobs |
| qstat | bjobinfo | get job info |


## Generic job submission script

```bash
[holder@scisub ~]$ cat test.sh 
#!/bin/bash
#BSUB -J my_test_job            # LSF job name
#BSUB -o my_test_job.%J.out     # Name of the job output file
#BSUB -e my_test_job.%J.error   # Name of the job error file

echo "this is a test"

sleep 15
```

# General cluster organizational differences

The grid computing system 
