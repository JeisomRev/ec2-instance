# Terraform AWS EC2 Project

This project uses Terraform to manage EC2 instances on AWS, with a GitHub Actions workflow for automatic initialization.

## Configuration

The `main.tf` file contains a simple Terraform configuration to manage an EC2 instance on AWS with the following spects:
- A t2.micro EC2 instance with Amazon Linux 2
- The instance is tagged with the name "ExampleInstance"

## GitHub Actions Workflow

The GitHub Actions workflow (`terraform-init.yml`) automatically initializes Terraform when a push is made to the main branch or a pull request is created.

### Required Secrets

The workflow requires the following secrets to be configured in the GitHub repository:

- `AWS_ACCESS_KEY_ID`: Your AWS access key ID
- `AWS_SECRET_ACCESS_KEY`: Your AWS secret access key

## Usage

1. Clone this repository.
2. Ensure you have Terraform installed.
3. Configure your AWS credentials locally.
4. Run the following commands:
`terraform init`
`terraform plan`
`terraform apply`
`terraform destroy` if necessary