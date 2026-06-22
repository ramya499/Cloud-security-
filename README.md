Intern Details
Intern ID: CITS3621
Name:Ramya Devi.R
Duration: 4 Weeks
Project Name
Cloud Security Auditor for AWS
Project Scope
This project simulates an AWS Cloud Security Auditor that checks cloud resources for common security misconfigurations. The system analyzes AWS services such as IAM, S3, EC2 Security Groups, and RDS databases to identify potential security risks and generate audit findings.
Technologies Used
Python
AWS SDK (Boto3)
JSON
ThreadPoolExecutor
Logging
Google Colab
AWS IAM
AWS S3
AWS EC2
AWS RDS
Features
Audits IAM Root Account MFA status
Checks S3 Bucket Public Access settings
Detects risky EC2 Security Group rules
Verifies RDS Storage Encryption
Generates security findings report
Parallel auditing for faster scanning
Project Workflow
Connect to AWS Account
Retrieve Cloud Resource Information
Analyze Security Configurations
Identify Vulnerabilities
Generate Security Findings Report
Display Audit Results
How to Run
1. Install Required Libraries
Bash
pip install boto3
2. Configure AWS Credentials
Python
import os

os.environ["AWS_ACCESS_KEY_ID"] = "YOUR_ACCESS_KEY"
os.environ["AWS_SECRET_ACCESS_KEY"] = "YOUR_SECRET_KEY"
os.environ["AWS_DEFAULT_REGION"] = "us-east-1"
3. Run the Python Script
Execute the Cloud Security Auditor script in Google Colab or Python.
4. View Audit Findings
The tool will display detected security issues and recommendations.
[
  {
    "Service": "IAM",
    "Severity": "CRITICAL",
    "Resource": "Root Account",
    "Issue": "Root account does not have MFA enabled."
  },
  {
    "Service": "S3",
    "Severity": "HIGH",
    "Resource": "prod-user-data-backup",
    "Issue": "Public Access Block is not fully enabled."
  },
  {
    "Service": "EC2/VPC",
    "Severity": "HIGH",
    "Resource": "Security Group",
    "Issue": "Unrestricted inbound access detected."
  }
]
Sample Findings
JSON
Future Improvements
Real-time AWS monitoring
Integration with AWS Security Hub
Automatic remediation of findings
Dashboard for visualization
Email and Slack alerts
Compliance checks (ISO 27001, PCI-DSS, SOC 2)
Conclusion
This project demonstrates how cloud security auditing can be automated using Python and AWS services. By continuously monitoring cloud resources and identifying security weaknesses, organizations can improve their security posture, reduce risks, and maintain compliance with industry standards.
