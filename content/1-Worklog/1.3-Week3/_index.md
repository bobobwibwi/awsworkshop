---
title: "Week 3 Worklog - Module 3: Advanced Amazon VPC Networking"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Weekly Theme

Build a customized virtual network architecture, control routing traffic, and allow Private Subnets to communicate securely with the Internet.

### Weekly Objectives

* Build a Custom VPC by dividing IP ranges (CIDR blocks).
* Allocate Route Tables for Public and Private Subnets.
* Deploy a NAT Gateway to securely pull system updates.

### Task Schedule

| Date | Day | Task Description | Lab / Project |
|---|---|---|---|
| 04/05/2026 | Monday | Perform IP address planning. Initialize a Custom VPC containing both Public and Private Subnets. | [Lab 000006 - Build Advanced VPC](https://000006.awsstudygroup.com) |
| 05/05/2026 | Tuesday | Configure an Internet Gateway (IGW). Edit the Route Table for the Public Subnet to route traffic to the IGW. | [Lab 000006 - Build Advanced VPC](https://000006.awsstudygroup.com) |
| 06/05/2026 | Wednesday | Create EC2 instances acting as Frontend (Public) and Backend (Private) to test network tiering. | Cloud Lab Environment |
| 07/05/2026 | Thursday | Allocate an Elastic IP. Create a NAT Gateway in the Public Subnet and point the Private Subnet's Route Table to the NAT. | [Lab 000007 - NAT Gateway & Routing](https://000007.awsstudygroup.com) |
| 08/05/2026 | Friday | Troubleshooting: Run ping tests from the Backend instance to the Internet via NAT Gateway, trace route traffic. | Troubleshooting |

### Expected Outcomes

* Complete an isolated network infrastructure lab with high security.
* Ensure internal servers remain completely invisible to the Internet while still being able to pull patches.

### Week 3 References

* [Lab 000006 - Design advanced virtual network Amazon VPC](https://000006.awsstudygroup.com)
* [Lab 000007 - Set up secure routing with NAT Gateway](https://000007.awsstudygroup.com)