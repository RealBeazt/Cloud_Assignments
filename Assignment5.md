# Assignment - 5
## Write IaC using terraform to create EC2 machine on AWS or azure or google cloud. (Compulsory to use Input and output variable files)

>Name: Aman Narnaware
>
>Roll: 322005
>
>Batch: B1
>
>PRN: 22110404

### 1.  What is Terraform?

Terraform is an open-source infrastructure as code (IaC) tool developed by HashiCorp. It enables users to define and provision data center infrastructure using a declarative configuration language. Essentially, Terraform allows you to manage and automate the provisioning of cloud, on-premises, or hybrid infrastructure resources such as virtual machines, networks, storage, and more.

### 2. Step-by-step screenshot to install and configure Terraform.

-  Download Terraform from official [hashicorp](https://developer.hashicorp.com/terraform/install#windows) website and extract the files.

   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/25e330ee-1128-46dd-9858-af6ff686d36e)

-  Add Terraform in path environment variable.

   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/59a1262c-584e-4818-adf0-67a1c92c50c2)

-  Check for installation.

   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/5c4d92cd-fcff-46d5-9fc6-e794473ca5cf)

### 3. Terraform script to create Infrastructure on any cloud platform (AWS or Azure or Google)

-  Script to create 2 ec2 instances.

```
# Provider Configuration
provider "aws" {
  region = "ap-south-1" # Change to your desired region
}

# Resource Configuration
resource "aws_instance" "example_instance1" {
  ami           = "ami-001843b876406202a" # Change to your desired AMI
  instance_type = "t2.micro"              # Change to your desired instance type
  tags = {
    Name = "ExampleInstance1"
  }
}

resource "aws_instance" "example_instance2" {
  ami           = "ami-001843b876406202a" # Change to your desired AMI
  instance_type = "t2.micro"              # Change to your desired instance type
  tags = {
    Name = "ExampleInstance2"
  }
}

```

-   Use `terraform init` command to initialize terraform.

    ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/5eacb355-53d5-4272-b728-ad684bf2700d)

-   Use `terraform apply` to apply those configurations.

    ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/16da6151-8d3c-4166-b155-4ef4d066d886)

-   You can log into AWS console to confirm the ec2 instances.

    ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/e0fcbf18-f5c4-45cf-aa02-07bf4808cb34)

