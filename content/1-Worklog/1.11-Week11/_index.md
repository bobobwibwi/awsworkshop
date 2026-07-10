---
title: "Week 11 Worklog - Final Project Implementation"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Weekly Topic

Get hands-on: Implement infrastructure and configure the actual system on AWS based on the approved Proposal.

### Weekly Objectives

* Deploy a secure core network architecture (VPC, Subnets, Security Groups).
* Build Compute and Database tiers ensuring High Availability.
* Integrate security protection and monitoring mechanisms for the system.

### Work Schedule

| Date | Day | Task Content | Lab / Project |
|---|---|---|---|
| 29/06/2026 | Monday | Initialize Custom VPC for the project. Partition IPs strictly, configure Internet Gateway and NAT Gateway. | Project Execution |
| 30/06/2026 | Tuesday | Configure the Database tier (RDS) completely isolated in Private Subnets, set up Security Group to only allow internal IPs. | Project Execution |
| 01/07/2026 | Wednesday | Package OS AMI, create Launch Template, and set up Auto Scaling Group integrated with ALB. | Project Execution |
| 02/07/2026 | Thursday | Integrate monitoring: Enable CloudWatch, configure SNS to send email notifications when the system shows signs of overload. | Project Execution |
| 03/07/2026 | Friday | Comprehensive testing: Simulate server failure to test the auto-recovery capability of the Auto Scaling Group. | System Testing |

### Expected Results

* Project infrastructure successfully deployed, running smoothly according to the architecture diagrams.
* System designed with a 'secure-by-design' mindset, meeting requirements for network security and high availability.

### Week 11 References

* Personal Project architecture design (Proposal).
* AWS Well-Architected Framework documentation.
