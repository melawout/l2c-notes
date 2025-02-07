# What is IAC with Terraform?


## What is Terraform?
- Terraform is an open-source infrastructure as code (IAC) software tool.
- Created by HashiCorp, it allows users to define and provision data center infrastructure using a high-level configuration language.
- Terraform supports various cloud providers, including AWS, Azure, Google Cloud, and many others.
- It enables the automation of infrastructure management, reducing manual intervention and potential errors.

## State Management
- Terraform keeps track of your real infrastructure in a state file.
- The state file acts as a source of truth for your environment.
- Terraform uses the state file to determine the changes needed to match your configuration.

## Collaboration
- Terraform allows collaboration on infrastructure with remote state backends.
- HCP Terraform (free for up to five users) enables secure state sharing with teammates.
- Provides a stable environment for Terraform to run in.
- Prevents race conditions when multiple people make configuration changes simultaneously.

## Integration with Version Control Systems (VCS)
- Connect HCP Terraform to VCSs like GitHub, GitLab, etc.
- Automatically propose infrastructure changes when committing configuration changes to VCS.
- Manage infrastructure changes through version control, similar to application code.

