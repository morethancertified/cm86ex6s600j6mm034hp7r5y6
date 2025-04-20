**Ticket Type:** Task  
**Title:** Terraform TFVars with AWS VPC  
**Project:** Cloud Infrastructure Deployment  
**Assignee:** You  
**Reporter:** Derek Morgan  
**Priority:** High  
**Labels:** Terraform, AWS, Variables, TFVars, VPC  
**Epic Link:** AWS Infrastructure Expansion  
**Sprint:** Sprint 01/Tfvars

**Lab Setup**

This lab uses Localstack to simulate an AWS environment. Localstack is already preinstalled in your environment. You don't need keys or to configure the provider. If you'd like to use your own account, feel free to specify your provider configuration and run `unset aws` and `unset terraform` to decouple them from Localstack.

**Description:**

Your team needs to set up Virtual Private Clouds (VPCs) in AWS for different environments. These VPCs need to be configured in such a way that all their attributes are modular and their values are stored in a `variables.tf` file. These variable definitions need to be added to variable definitions files in order to deploy environments with different attributes dynamically.

**Acceptance Criteria:**

> **Note:** If the `terraform validate` command fails, all tasks in the lab will fail!

1. Create two files that define variables needed to deploy a `development` and a `production` VPC environment.   
2. The variables needed are:   
   1. `project` - The project name for the VPC  
   2. `env` - The environment (dev or prod)  
   3. `enable_dns_hostnames` - Whether DNS hostnames are enabled  
   4. `cidr_block` - The CIDR block for the VPC  
3. Within the two files, create values for these variables that make sense for each environment (e.g., smaller CIDR for dev, larger for prod). 

**Implementation Notes:**

Feel free to use code from previous labs. The values aren't as important as the concepts. 

- <a href="https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc" target="_blank">AWS VPC Resource Documentation</a>  
- <a href="https://developer.hashicorp.com/terraform/language/values/variables" target="_blank">Terraform Variables Documentation</a>  
- <a href="https://developer.hashicorp.com/terraform/language/values/variables#variable-definitions-tfvars-files" target="_blank">Terraform Variable Definitions Files Documentation</a>
