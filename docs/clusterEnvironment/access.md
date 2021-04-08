---
layout: default
title: Accessing the cluster
parent: Cluster Environment
has_toc: true
---

# Cluster access 
{: .no_toc }

The BSC LPC is behind the PSOM fire wall.
*ssh* access is supported through *scisub.pmacs.upenn.edu*.

```bash
ssh -XY holder@sciscub.pmacs.upenn.edu
```


## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Installed Software

PMACS uses modules for most installed software.

Run

```bash
module avail
```

to list the software installed.

Login to [the PMACS helpdesk](https://helpdesk.pmacs.upenn.edu) and click on 
*Need Help? Submit a ticket* then *Systems* to submit a help ticket.

## Login nodes

Once logged into *scisub.pmacs.upenn.edu*, you can login to one of the interactive BSC LPC nodes with

```
$ QUEUE=bsc ibash
```
for normal shell access.

## X11 forwarding

Use *xbash* to tunnel X connections

```
$ QUEUE=bsc xbash
$ xeyes
```

Currently there is no x2go equivalent for X11 forwarding.
