# Terraform AWS Infrastructure Project

This Terraform project provisions AWS infrastructure including a VPC, subnets, EC2 instance, and security groups.

## Resources
- VPC
- Public & Private Subnets
- EC2 Instance
- IAM Role & Policy
- Security Group

## Steps

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/aws-terraform-project.git
   cd aws-terraform-project
2. **Modify terraform.tfvars**

Update the my_ip variable with your public IP address to allow SSH access.
```bash
my_ip = "95.168.105.29/32"
```

3. ### Initialize Terraform
Initialize your Terraform workspace by running the following command:
```bash
terraform init
```

4. #### Apply the configuration
After initialization, apply the configuration to provision resources.
```bash
terraform apply
```

5. ##### Check the output
After Terraform applies the configuration, it will display the public IP of the EC2 instance:
```bash
Apply complete! Resources: 11 added, 0 changed, 0 destroyed.

Outputs:

ec2_public_ip = "xx.xx.xx.xx"
```

### Security Consideration
SSH access is restricted to your public IP for security. Make sure to replace my_ip with your actual public IP to prevent unauthorized access.
