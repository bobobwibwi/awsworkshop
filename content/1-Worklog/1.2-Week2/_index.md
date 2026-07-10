---
title: "Week 2 Worklog - Module 2: Amazon EC2 & EBS Cloud Computing"
date: 2026-04-24
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Weekly Theme

Deploy, configure Amazon EC2 virtual servers, and allocate EBS storage.

### Weekly Objectives

* Initialize and securely connect to an EC2 Linux server via SSH.
* Configure Inbound/Outbound rules in Security Groups.
* Expand storage capacity with Elastic Block Store (EBS) volumes.

### Task Schedule

| Date | Day | Task Description | Lab / Project |
|---|---|---|---|
| 27/04/2026 | Monday | Launch the first t2.micro instance. Practice secure SSH connection via Key Pair (.pem file). | [Lab 000004 - Introduction to Amazon EC2](https://000004.awsstudygroup.com) |
| 28/04/2026 | Tuesday | Learn about Security Groups. Open port 22 (SSH) for personal IP and port 80 (HTTP) to the Internet. | [Lab 000004 - Introduction to Amazon EC2](https://000004.awsstudygroup.com) |
| 29/04/2026 | Wednesday | Write a User Data script to automatically install Apache Web Server upon EC2 startup. Test web access. | Scripting / User Data |
| 30/04/2026 | Thursday | Create a new EBS Volume, attach it to the running EC2 instance, and execute Linux commands to mount the partition. | [Lab 000005 - Storage with Amazon EBS](https://000005.awsstudygroup.com) |

### Expected Outcomes

* Successfully host a basic web page on an EC2 instance.
* Tighten the security perimeter at the network layer (Security Group).
* Master the allocation and mounting of virtual EBS hard drives without damaging the OS.

### Week 2 References

* [Lab 000004 - Introduction and configuration of Amazon EC2](https://000004.awsstudygroup.com)
* [Lab 000005 - Storage space management with Amazon EBS](https://000005.awsstudygroup.com)