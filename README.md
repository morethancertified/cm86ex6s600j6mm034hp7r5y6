**Ticket Type:** Task  
**Title:** Terraform TFVars  
**Project:** Version Control System Deployment  
**Assignee:** You  
**Reporter:** Derek Morgan  
**Priority:** High  
**Labels:** Terraform, GitHub, Variables, Validation  
**Epic Link:** GitHub Expansion  
**Sprint:** Sprint 01/Tfvars

**Description:**

A repository is needed for development code. This repository needs to be configured in such a way that all its attributes are modular and their values are stored in a `variables.tf` file. These variable definitions need to be added to variable definitions files in order to deploy environments with different attributes dynamically. 

**Acceptance Criteria:**

> **Note:** If the `terraform validate` command fails, all tasks in the lab will fail!

1. Create two files that define variables needed to deploy a `development` and a `production` repository.   
2. The variables needed are   
   1. `project`   
   2. `env`  
   3. `auto_init`  
   4. `gitignore`  
3. Within the two files, create values for these variables that make sense for each environment. 

**Implementation Notes:**

Feel free to use code from previous labs. The values aren’t as important as the concepts. 

\- [GitHub Provider Docs](https://registry.terraform.io/providers/integrations/github/latest/docs)  
- <a href="https://developer.hashicorp.com/terraform/language/values/variables" target="_blank">Terraform Documentation</a>  
- <a href="https://developer.hashicorp.com/terraform/language/values/variables#variable-definitions-tfvars-files" target="_blank">Terraform Documentation</a>
