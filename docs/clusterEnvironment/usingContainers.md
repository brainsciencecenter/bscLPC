---
layout: default
title: Containerized software
parent: Cluster Environment
has_children: false
has_toc: true
---
# Singularity
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Singularity support on the LPC

[Singularity](https://sylabs.io/docs/) is a containerization system designed for scientific and cluster
computing environments. It has good interoperability with Docker for most use
cases. 


## Building Singularity images from Docker images

There is a dedicated Singularity build machine, accessible from sciget. Connect
to it and load Singularity with

```
$ ssh singularity01
$ module load DEV/singularity
```

You can then build Singularity images from DockerHub, or locally.
 

## Running Singularity containers 
