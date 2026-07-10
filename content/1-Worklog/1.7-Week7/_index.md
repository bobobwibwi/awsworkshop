---
title: "Week 7 Worklog - Module 7: CloudWatch Monitoring & Log Analysis"
date: 2026-05-29
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Weekly Theme

Use monitoring tools to track system health and set up automated incident alert scenarios.

### Weekly Objectives

* Monitor resource graphs using CloudWatch Metrics.
* Integrate Simple Notification Service (SNS) to receive Email Alerts.
* Collect VPC Flow Logs to assist in tracing suspicious network behavior.

### Task Schedule

| Date | Day | Task Description | Lab / Project |
|---|---|---|---|
| 01/06/2026 | Monday | Access CloudWatch Metrics, create a Dashboard to monitor CPU and Network In/Out metrics of the EC2 cluster. | CloudWatch Basics |
| 02/06/2026 | Tuesday | Create a Topic on Amazon SNS and register a personal email. Link SNS with a Billing Alarm for cost alerts. | [Lab 000027 - SNS & Alarms](https://000027.awsstudygroup.com) |
| 03/06/2026 | Wednesday | Create a CloudWatch Alarm to warn when the application experiences abnormal load and automatically send incident notification emails. | [Lab 000027 - SNS & Alarms](https://000027.awsstudygroup.com) |
| 04/06/2026 | Thursday | Enable VPC Flow Logs. Analyze network logs to filter out IP addresses rejected by the Security Group. | [Lab 000028 - VPC Flow Logs](https://000028.awsstudygroup.com) |

### Expected Outcomes

* Gain full control over the system status, automating Email Alerts when abnormal fluctuations occur.
* Know how to use network logs to analyze and conduct preliminary investigations of information security risks (like port scanning, probing attacks).

### Week 7 References

* [Lab 000027 - Automated Alerts with Amazon CloudWatch & SNS](https://000027.awsstudygroup.com)
* [Lab 000028 - Collect and Analyze Network Traffic with VPC Flow Logs](https://000028.awsstudygroup.com)