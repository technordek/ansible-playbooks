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
