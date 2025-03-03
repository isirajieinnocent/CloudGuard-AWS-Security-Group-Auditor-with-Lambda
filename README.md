<h1> Project Overview </h1>

This project is a Security Group Audit Tool designed to enhance the security posture of an AWS environment. It programmatically checks AWS security groups for potentially risky inbound rules (e.g., unrestricted access from 0.0.0.0/0) and sends real-time alerts via AWS SNS (Simple Notification Service).

<h1> The Architecture </h1> 

![image](https://github.com/user-attachments/assets/73f466ca-6ec5-4680-b8a4-179fa44d3db3)

<h1> Solution Overview </h1>

**Automated Security Check:**

The AWS Lambda function iterates through all security groups in the AWS account.

Examines inbound rules (ip_permissions) for configurations that allow unrestricted traffic.

**Real-Time Alerts:**

***When a risky rule is detected:***

Logs a detailed warning message about the rule and its associated security group.

Publishes an alert to an SNS topic, notifying administrators via email, SMS, or other channels.

**Serverless Architecture:**

Fully managed and scalable, leveraging AWS Lambda with no server infrastructure required.

**Customizable:**

Can be extended to include additional rule checks or automate remediation of risky configurations.

<h1> Key Technologies </h1>

AWS Lambda: Serverless execution for automated security checks.

**AWS EC2 SDK (Boto3):** Queries and analyzes security groups.

**AWS SNS:** Sends real-time alerts to administrators.

<h1> Impact  </h1>

**Proactive Risk Management:** Identifies and flags misconfigured security groups, minimizing exposure to unauthorized access and potential data breaches.

**Cost-Effective Monitoring:** Leverages AWS Lambda for cost-efficient, on-demand execution.

**Seamless Integration:** Integrates with existing workflows via AWS SNS for immediate response.

<h1> Key Achievements </h1>

Designed a serverless solution to automate security group auditing.

Implemented real-time alerting using AWS SNS for immediate risk notification.

Enhanced cloud security posture by identifying and flagging risky configurations.

This project highlights my expertise in AWS serverless architecture, cloud security best practices, and Python programming. It demonstrates my ability to build scalable, cost-effective solutions for proactive risk management in cloud environments.
