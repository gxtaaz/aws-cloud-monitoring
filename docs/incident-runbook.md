# Incident Runbook: High CPU Utilization

## 1. Incident Overview
A CloudWatch alarm is configured to detect when the average CPU utilization of the monitored EC2 instance exceeds 70%.

## 2. Monitoring Configuration
- Cloud service: Amazon EC2
- Operating system: Ubuntu Linux
- Monitoring service: Amazon CloudWatch
- Metric: CPUUtilization
- Alarm name: High-CPU-CloudOps-Alarm
- Notification service: Amazon SNS
- Notification method: Email

## 3. Investigation Procedure
1. Open the CloudWatch alarm and review its current state.
2. Check the CPU utilization graph and identify any unusual increases.
3. Connect to the Ubuntu server using SSH.
4. Run `uptime` to inspect system load.
5. Run `top` to identify processes consuming CPU.
6. Investigate the cause of high utilization before taking corrective action.

## 4. Response Procedure
1. Identify unnecessary or resource-intensive processes.
2. Stop test workloads when they are no longer required.
3. Investigate unexpected CPU usage before stopping important processes.
4. Escalate persistent or unexplained issues when necessary.

## 5. Recovery Verification
1. Confirm that CPU utilization has decreased.
2. Check whether the CloudWatch alarm returns to the OK state.
3. Review alarm history and verify email delivery if a notification was triggered.

## 6. Preventive Measures
- Monitor CPU utilization trends.
- Review alarm thresholds periodically.
- Investigate recurring CPU spikes.
- Verify that notification subscriptions remain active.

## 7. Evidence and Documentation
Add screenshots of the EC2 instance, SNS subscription, CloudWatch alarm, and any email alerts or alarm state transitions that were actually observed.
