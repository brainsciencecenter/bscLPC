---
layout: default
title:  Support
has_children: false
has_toc: true
nav_order: 3
---

# Troubleshooting

## If you can't connect

## Ensure you are logged in to the correct node

There are three access points at {node}.pmacs.upenn.edu, where {node} is

* transfer - no shell access, scp / sftp only for uploading or downloading data.
* sciget - shell access + Internet, git, other data transfer (sciget7 is a CentOS 7 node with similar access but is acciable from the Internet).
* scisub - job submission. bsub, ibash, xbash, only work from here.

None of these login nodes should be used for computationally intensive jobs, and
most of the data processing software is unavailable on these machines. To run
something like FSL or FreeSurfer interactively, request a compute slot with
ibash or xbash.


# Community resources

## UPenn MRI Slack

The UPenn MRI slack channel is:

```bash
upennmri.slack.com
```
and is the expected place for messaging about doing MRIs at Penn, as well as flywheel, and the BSC PMACS cluster

# PMACS support

## Password reset

You can reset your PMACS password at

https://reset.pmacs.upenn.edu/showLogin.cc

## Opening a ticket

https://helpdesk.pmacs.upenn.edu

Select "Need Help? Report it!" then "Systems".  There are lots of options you may fill in when submitting a help ticket.  The CC option is probably the most useful.

## Additional computing resources

