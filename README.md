# AWS Cloud Monitoring and Incident Alerting System

## Overview
A beginner-friendly cloud operations project that monitors an Ubuntu EC2 instance using Amazon CloudWatch and sends email notifications through Amazon SNS when CPU utilization exceeds a configured threshold.

## Architecture
EC2 (Ubuntu) → CloudWatch CPU Metric → CloudWatch Alarm → Amazon SNS → Email Notification

## Technologies
- Amazon EC2
- Ubuntu Linux
- Amazon CloudWatch
- Amazon SNS
- SSH and Linux command-line tools
- Git and GitHub

## Implementation
1. Used an Ubuntu EC2 instance as the monitored server.
2. Configured an SNS topic and confirmed an email subscription.
3. Created a CloudWatch alarm for high CPU utilization.
4. Tested the alarm using a temporary CPU workload.
5. Documented investigation, response, and verification procedures in an incident runbook

## Results
- EC2 instance: [Add actual instance details]
- Alarm threshold: 70% average CPU utilization
- Email notification: [Not yet verified]

## Incident Response
See [docs/incident-runbook.md](docs/incident-runbook.md).

## Security and Cost Management
- Restricted SSH access to the administrator's IP address.
- Used temporary CPU load only for testing.
- Reviewed AWS resources and cleaned up resources after testing.

## Learning Outcomes
Practiced basic AWS monitoring, Linux administration, alert configuration, incident investigation, and operational documentation.
