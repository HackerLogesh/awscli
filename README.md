# awscli
📌 Configure AWS CLI:

bash
Copy
Edit
aws configure
You'll be prompted for:

AWS Access Key ID

AWS Secret Access Key

Default region (e.g., us-east-1)

Output format (json, table, or text)

📦 Common AWS CLI Commands
✅ S3 – Simple Storage Service

bash
Copy
Edit
# List buckets
aws s3 ls

# Upload a file
aws s3 cp file.txt s3://my-bucket/

# Sync local folder to S3
aws s3 sync ./local-folder s3://my-bucket/
✅ EC2 – Virtual Servers

bash
Copy
Edit
# List EC2 instances
aws ec2 describe-instances

# Start an instance
aws ec2 start-instances --instance-ids i-0123456789abcdef0

# Stop an instance
aws ec2 stop-instances --instance-ids i-0123456789abcdef0
✅ IAM – Identity & Access Management

bash
Copy
Edit
# List IAM users
aws iam list-users

# Create a new user
aws iam create-user --user-name newuser
✅ VPC – Virtual Private Cloud

bash
Copy
Edit
# List all VPCs
aws ec2 describe-vpcs

# Create a VPC
aws ec2 create-vpc --cidr-block 10.0.0.0/16
✅ CloudFormation – IaC Deployment

bash
Copy
Edit
# Deploy a CloudFormation stack
aws cloudformation deploy --template-file template.yaml --stack-name mystack
✅ Lambda – Serverless Functions

bash
Copy
Edit
# List all Lambda functions
aws lambda list-functions
🧠 Power Tips
💡 Use --profile for multiple accounts:

bash
Copy
Edit
aws s3 ls --profile dev
💡 Use --region for region-specific tasks:

bash
Copy
Edit
aws ec2 describe-instances --region us-west-2
💡 Automate with bash + jq for powerful scripting!
