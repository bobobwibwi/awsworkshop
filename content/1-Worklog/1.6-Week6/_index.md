---
title: "Week 6 Worklog - Module 6: ELB Load Balancing & Auto Scaling"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Weekly Theme

Solve performance bottlenecks: Automatically balance traffic and scale the number of servers based on actual load.

### Weekly Objectives

* Configure an Application Load Balancer (ALB) to coordinate traffic.
* Package an AMI and create standard Launch Templates.
* Build an Auto Scaling Group (ASG) to support automated Scale Out/Scale In.

### Task Schedule

| Date | Day | Task Description | Lab / Project |
|---|---|---|---|
| 25/05/2026 | Monday | Create an Amazon Machine Image (AMI) from an EC2 instance pre-installed with stable web source code. | [Lab 000019 - Package AMI](https://000019.awsstudygroup.com) |
| 26/05/2026 | Tuesday | Create a Launch Template based on the generated AMI, define the instance type, key pair, and shared security group. | [Lab 000021 - Launch Templates](https://000021.awsstudygroup.com) |
| 27/05/2026 | Wednesday | Set up an Application Load Balancer (ALB). Configure a Target Group and Health Checks to identify active servers. | [Lab 000020 - Elastic Load Balancing](https://000020.awsstudygroup.com) |
| 28/05/2026 | Thursday | Initialize an Auto Scaling Group (ASG) attached to the ALB. Write a Scaling Policy to automatically add servers if CPU exceeds 70%. | [Lab 000022 - Auto Scaling Setup](https://000022.awsstudygroup.com) |
| 29/05/2026 | Friday | Use Apache Benchmark to run stress tests to increase server load, monitor logs to see ASG spawn additional EC2s. | Stress Testing |

### Expected Outcomes

* Ensure the system maintains High Availability even if a server suddenly crashes.
* System capacity dynamically scales out during traffic storms and scales in during off-peak hours to optimize costs.

### Week 6 References

* [Lab 000020 - Distribute Traffic with Elastic Load Balancing](https://000020.awsstudygroup.com)
* [Lab 000022 - Automated Scaling with Auto Scaling Group](https://000022.awsstudygroup.com)