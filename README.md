Terraform Module to provision an AWS EC2 instance with the latest amazon linux 2023 ami and installed docker in it.

Not intended for production use. It is an example module.

It is just for showing how to create a publish module in Terraform Registry.

Usage:

```hcl

provider "aws" {
  region = "us-east-1"
}

module "docker_instance-2024" {
    source = "recep-instructor/docker-instanc-2024/aws"
    key_name = "clarusway"
}
```