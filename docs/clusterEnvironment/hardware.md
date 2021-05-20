---
layout: default
title: Hardware and storage
parent: Cluster Environment
has_toc: true
---

# Cluster computing and data storage
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Compute nodes

The BSC PMACS cluster has 9 compute nodes

Eight PowerEdge R640 Servers with:
+ 2 Intel Xeon Gold 6240R 2.4G processors with 24 cores each
+ 384GB of RAM and 8GB / core
+ 2TB of SSD local storage for scratch space
+ 10Gig Dual Ethernet ports
+ 1Gig Quad Ethernet ports

One Dell PowerEdge 640 with twice the RAM
+ 2 Intel Xeon Gold 6240R 2.4G processors with 24 cores each
+ 768GB of RAM and 16GB / core
+ 2TB of SSD local storage for scratch space
+ 10Gig Dual Ethernet ports
+ 1Gig Quad Ethernet ports

All nine nodes are housed in the Perlman School of Medicine's commercial-grade server room with redundant power supplies; UPS power backup systems; fire suppression system; and 24-hour restricted access and security. 

## Network storage

PMACS is currently providing 130TB of NFS storage for the BSSC Cluster.  The storage is redundant and backed up to tape. 

## Temporary storage

Each compute node has 2TB of SSD local storage for scratch space.
