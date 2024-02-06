# LAB PVT CISG FY2024Q2 - Nexus as Code

Welcome to our repository! In order for this code to work you MUST configure your Virtual Machine Manager (VMM) domain by updating the `vmm_domain.yaml` file and setting up your Terraform environment by creating a `variables.tf` file in the working directory. Follow the instructions below to ensure a smooth setup process.

## Configuration Instructions

### Step 1: Update the `vmm_domain.yaml` File

The `vmm_domain.yaml` file in the `data` folder contains critical configuration settings for your VMM domain. 
Uncomment the lines with ```#``` and change the ```<variable>``` parameters with the credentials

#### Why This Step Is Important

- Ensures your VMM domain is configured with the correct parameters.
- Helps avoid common configuration errors.
- Customizes the setup to meet your specific requirements.

### Step 2: Create Your `variables.tf` File

Terraform uses the `variables.tf` file to manage environment-specific values. Please create a file with the necessary inputs, replacing `<placeholder>` values with your actual data.

```hcl
variable "username" {
  default = "<username>"
  type    = string
}

variable "password" {
  default = "<password>"
  type    = string
}

variable "url" {
  default = "<url_apic>"
  type    = string
}

```

# Getting Help
If you encounter any issues or have questions, please open an issue in this repository or e-mail me lbertini@cisco.com, and we'll be happy to help.
