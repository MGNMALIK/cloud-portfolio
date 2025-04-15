# CloudWatch CPU Alarm Project (4/14/25)

This project demonstrates how to monitor EC2 CPU usage and trigger email alerts using CloudWatch and SNS.

## AWS Services Used

- EC2
- CloudWatch (for monitoring)
- SNS (for notifications)

## Steps Taken

1. Launched an EC2 instance (t2.micro)
2. Created an SNS topic and email subscription
3. Created a CloudWatch alarm for CPUUtilization > 70%
4. Simulated CPU load using `yes > /dev/null &`
5. Received alert via email when alarm was triggered

## Screenshots

### Alarm Triggered
![Alarm](./screenshots/cloudwatch-alarm.png)

### EC2 Instance
![EC2](./screenshots/ec2-instance-status.png)

### Email Alert
![Alert](./screenshots/sns-email-alert.png)

### CPU Load Test in SSH
![CPU Load Test](./screenshots/ssh-cpu-test.png)

## What I Learned

- How to set up proactive monitoring
- Using native tools for real-time alerts
- How to simulate stress testing in a cloud environment


