Terraform Workspaces - OSS

Those who adopt Terraform typically want to leverage the principles of DRY (Don't Repeat Yourself) development practices.
One way to adopt this principle with respect to IaC is to utilize the same code base for different environments (development, quality, production, etc.)

Workspaces is a Terraform feature that allows us to organize infrastructure by environments and variables in a single directory.

Terraform is based on a stateful architecture and therefore stores state about your managed infrastructure and configuration. 
This state is used by Terraform to map real world resources to your configuration, keep track of metadata, and to improve performance for large infrastructures.

The persistent data stored in the state belongs to a Terraform workspace. 
Initially the backend has only one workspace, called "default", and thus there is only one Terraform state associated with that configuration.

 1: Using Terraform Workspaces (Open Source)
 2: Create a new Terraform Workspace for Development State
 3: Deploy Infrastructure within the Terraform development workspace
 4: Changing between Workspaces
 5: Utilizing the ${terraform.workspace} interpolation sequence within your configuration
