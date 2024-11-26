Project Overview

The project is a Security Group Audit Tool designed to enhance the security posture of an AWS environment. It programmatically checks AWS security groups for potentially risky inbound rules, such as those allowing unrestricted access from all IP addresses (0.0.0.0/0). If such rules are found, the tool generates a warning and sends an alert via AWS SNS (Simple Notification Service).

Key Features
Automated Security Check:

The Lambda function iterates through all security groups in the AWS account.
It examines their inbound rules (ip_permissions) for configurations that allow unrestricted traffic.
Real-Time Alerts:

When a risky rule is detected, the function:
Logs a detailed warning message about the rule and its associated security group.
Publishes an alert to an SNS topic, which can notify administrators via email, SMS, or other channels.
Serverless Architecture:

Fully managed and scalable since it leverages AWS Lambda, requiring no server infrastructure.
Customizable:

The solution can be extended to include additional rule checks or to remediate risky configurations automatically.
Purpose and Value
Proactive Risk Management:

Identifying and flagging misconfigured security groups minimizes exposure to unauthorized access and potential data breaches.
Cost-Effective Monitoring:

The use of AWS Lambda ensures the solution is cost-efficient and only runs when triggered.
Integration with Existing Workflows:

By leveraging SNS, it seamlessly integrates into notification or ticketing systems for immediate response.
Technologies Used
AWS Lambda: For serverless execution.
AWS EC2 SDK (Boto3): To query and analyze security groups.
AWS SNS: For sending alerts to administrators.
This project demonstrates proficiency in AWS, serverless computing, and cloud security best practices, showcasing skills in Python programming, resource auditing, and real-time alerting systems. It is ideal for organizations prioritizing secure and automated cloud environments.
