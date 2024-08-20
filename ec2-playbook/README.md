# AWS EC2 Ansible Playbooks

## Prerequisites
- Ansible >= 2.9
- Python >= 3.6
- AWS CLI configured with necessary credentials
- boto3 installed (`pip install boto3`)

## Steps to install Prerequisites
- Install Ansible using (“sudo apt install ansible”) 
- Install boto and boto3 using (“sudo apt install python3-boto python3-boto3”). These are libraries required 
  for Ansible to interact with AWS. 
- Install Amazon  collection using ("ansible-galaxy collection install amazon.aws").This command will download 
  and install the amazon.aws collection from Ansible Galaxy, making it available for use in your Ansible 
  playbooks.If the command says its already installed its fine. 
- If not force install it using the  below command 
   ('ansible-galaxy collection install community.aws --force-with-deps') 
- Check the aws version and configure AWS using “aws configure” if it displays like below the install the 
  updated version. 
- Use below command to install the updated version . 
  "sudo apt-get install curl"(Install curl if you dont have it) 
  ('curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"') 
- A zip file will be downloaded use below command to unzip the file and install the updated version
   ('unzip awscliv2.zip  and sudo ./aws/install') 

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/technordek/ansible-playbooks.git

# Launching new instance via this playbook

When prompted by ansible playbook for launching an EC2 similar to other ec2 instances with same networking.

We can follow this format:

Enter the name for the new EC2 instance: nameofinstance
Enter the type for the new EC2 instance: t3.medium
Enter the EBS volume size in GB: 30
Enter the EBS volume type (e.g., gp2, io1, st1, sc1): gp3
Choose the OS for the EC2 instance (amazon_linux, ubuntu, centos): ubuntu
Enter the existing VPC ID (leave blank if not applicable): vpc-02815fe7d001d0224
Enter the public subnet ID (leave blank if not applicable): subnet-0581563a893bbcc73
Enter the private subnet ID (leave blank if not applicable): subnet-07460c9d948029599
Enter the security group ID (leave blank if not applicable): 
Enter the key name to use (leave blank if not applicable): nameofinstance-key
Enter the internet gateway ID to use (leave blank if not applicable): igw-0e34d32a90d06dfdf
Enter the route table ID to use (leave blank if not applicable): 
