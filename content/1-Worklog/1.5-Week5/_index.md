---
title: "Week 5 Worklog - Module 5: Amazon RDS Cloud Database"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Weekly Theme

Utilize Managed Database services to eliminate OS operational burden, focusing on data tier security.

### Weekly Objectives

* Initialize an Amazon RDS (MySQL/PostgreSQL) server safely in a Private Subnet.
* Ensure High Availability using the Multi-AZ option.
* Configure Security Groups to allow EC2 to read/write to the Database.

### Task Schedule

| Date | Day | Task Description | Lab / Project |
|---|---|---|---|
| 18/05/2026 | Monday | Initialize a DB Subnet Group consisting of Private Subnets spread across multiple AZs. | Network Configuration |
| 19/05/2026 | Tuesday | Create an Amazon RDS MySQL instance, configure the Master Password, and disable Public Access. | [Lab 000015 - Deploy Amazon RDS](https://000015.awsstudygroup.com) |
| 20/05/2026 | Wednesday | Set up RDS Security Group: Only accept port 3306 traffic coming from the EC2 Web Server's Security Group. | Network Security |
| 21/05/2026 | Thursday | From the EC2 instance, use a MySQL Client to test the connection to the RDS Endpoint. Create a Snapshot backup and clean up. | [Lab 000015 - Deploy Amazon RDS](https://000015.awsstudygroup.com) |

### Expected Outcomes

* The database is completely isolated and cannot be accessed directly from the Internet.
* Successfully communicate over a secure internal route between the Compute tier and the Database tier.

### Week 5 References

* [Lab 000015 - Initialize and Configure Amazon RDS](https://000015.awsstudygroup.com)