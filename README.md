# Platform Engineer - Tech Task

Welcome to the code challenge for the Platform Engineering role at Lean Tree. This challenge will give you an opportunity to showcase your skills in Terraform, Git, and Shell scripting, as well as your understanding of AWS resources. The challenge is divided into three parts, each focusing on a specific aspect.

Good luck! We're excited to see your solutions and how you tackle each part of the challenge.

## Part 1 - Terraform: Create AWS EC2 Instance

### Acceptance Criteria

1. Create an AWS EC2 Linux Ubuntu instance with the following specifications:
   - Instance type: t2.micro
   - Use the default VPC and subnet provided by AWS
2. Attach two tags to the EC2 instance:
   - Tag 1: Key = "Name", Value = [Choose any appropriate name]
   - Tag 2: Key = "Environment", Value = [Choose any appropriate environment]
3. Define a security group resource for the EC2 instance with the following requirements:
   - Allow inbound traffic on port 22 (SSH) from any source IP address
   - Allow outbound traffic to any destination IP address on all ports

### Instructions

1. Write the Terraform code to create an AWS EC2 instance and define the necessary resources according to the acceptance criteria.
2. Provide clear comments in your code, or verbally explain the purpose and functionality of each resource or configuration block.
3. Deploy your Terraform code to the Lean Tree Interviews AWS Account using credentials supplied during the interview.

## Part 2 - Terraform: Refactoring

### Acceptance Criteria

1. Refactor the Terraform code from Part 1 to a reusable opinionated Terraform module.
2. The refactored code should still create all the resources from Part 1, and:
   - Allows the Instance Type to be parameterised
   - Allows the Environment Tag to be parameterised
3. The AWS resources should not be modified during the refactoring process.

### Instructions

1. Modify the Terraform code to meet the necessary acceptance criteria.
2. Provide clear comments in your code, or verbally explain the purpose and functionality of each resource or configuration block.
3. Deploy your Terraform code to the Lean Tree Interviews AWS Account using credentials supplied during the interview.

## Part 3 - Shell Scripting: Recursive Text Search

### Acceptance Criteria

Write a Shell Script that:

1. Searches for a specific text pattern within all files of a given file type.
2. Takes in two command-line arguments:
   - Argument 1: The specific text pattern to search for (e.g., "ec2").
   - Argument 2: The file type to search within (e.g., ".tf").
3. Outputs the File Paths of all matching files.
4. Outputs the Total Count of files found.
5. Handles cases where no matching files are found gracefully, displaying an appropriate message.

### Instructions

1. Choose a shell scripting language (e.g., Bash, Zsh) that you prefer to use for this task.
2. Write a shell script that meets the acceptance criteria mentioned above.
3. Test your script locally to ensure it is working as expected.
4. Demonstrate the functionality of your script by searching for the text pattern "ec2" within all `.tf` files generated as part of the code written in Part 1 and Part 2.
