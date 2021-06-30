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
#!/bin/bash
#BSUB -J my_test_job            # LSF job name
#BSUB -o my_test_job.%J.out     # Name of the job output file
#BSUB -e my_test_job.%J.error   # Name of the job error file   

# if you want to receive e-mail notifications on a non-default address
#BSUB -u holder@upenn.edu  # *** make sure to set this to your email address
### -- send notification at start --
#BSUB -B
### -- send notification at completion --
#BSUB -N

echo "this is a test"
sleep 15

```

Run and check with ```bsub``` and ```bjobs```

```bash
[holder@scisub ~]$ bsub /home/holder/test.sh
Job <9375077> is submitted to queue <bsc_normal>.
[holder@scisub ~]$ bjobs 9375077
JOBID      USER    STAT  QUEUE      FROM_HOST   EXEC_HOST   JOB_NAME   SUBMIT_TIME
9375077    holder  RUN   bsc_normal scisub      bsc04       *r/test.sh Jun 29 16:03
[holder@scisub ~]$ bjobs 9375077
JOBID      USER    STAT  QUEUE      FROM_HOST   EXEC_HOST   JOB_NAME   SUBMIT_TIME
9375077    holder  RUN   bsc_normal scisub      bsc04       *r/test.sh Jun 29 16:03
[holder@scisub ~]$ bjobs 9375077
JOBID      USER    STAT  QUEUE      FROM_HOST   EXEC_HOST   JOB_NAME   SUBMIT_TIME
9375077    holder  DONE  bsc_normal scisub      bsc04       *r/test.sh Jun 29 16:03

```

when the job is complete, email is sent to holder@upenn.edu.

Had the job been submitted with:

```bash
bsub < test.sh
```
output files would be created and the email would not includ any output.

### Supressing completion emails

# General cluster organizational differences

The grid computing system 
