# **Important note** 

Note that every region has a different AMI ID. the AMI IDs keeps changing, so you must ensure that you use the latest AMI ID from the AWS console.

provider "aws" {
  region     = "us-west-2"
  access_key = "PUT-YOUR-ACCESS-KEY-HERE"
  secret_key = "PUT-YOUR-SECRET-KEY-HERE"
}

resource "aws_instance" "myec2" {
   ami = "ami-082b5a644766e0e6f"
   instance_type = "t2.micro"
}




Commands:

```r
$ terraform init` *to initiate terraform*

```r
$ terraform plan *to get nformation on what exactly terraform is about to create*
```
```r
$ terraform apply *to actually create the resource written in the configuration.*
```
  
***kindly note that is very important to run the Plan before the apply each time to see what will happen in advance!!***
