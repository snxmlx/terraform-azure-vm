# Terraform Azure VM Setup

## Overview
This repository provides a Terraform configuration to set up a virtual machine (VM) in Microsoft Azure. It is designed to simplify the provisioning process by defining infrastructure as code.

## Features
- Automates the creation of an Azure Virtual Machine.
- Uses Terraform for infrastructure provisioning.
- Includes configuration for providers, variables, and outputs.

## Repository Structure
The repository contains the following files:

- **main.tf**: Defines the core resources for the Azure VM setup.
- **providers.tf**: Configures the Azure provider and any required plugins.
- **variables.tf**: Specifies input variables to customize the deployment.
- **outputs.tf**: Defines output values to display after the infrastructure is provisioned.
- **.gitignore**: Specifies files and directories to be ignored by Git.

## Prerequisites
Before using this repository, ensure you have the following:
1. An active [Microsoft Azure account](https://azure.microsoft.com/).
2. [Terraform installed](https://www.terraform.io/downloads) on your local machine.
3. Azure CLI installed and authenticated (`az login`).

## Usage
Follow these steps to deploy an Azure VM using this repository:

1. Clone the repository:
   ```bash
   git clone https://github.com/snxmlx/terraform-azure-vm.git
   cd terraform-azure-vm
   ```

2. Initialize Terraform:
   ```bash
   terraform init
   ```

3. Review and customize variables in `variables.tf` or provide them via a `terraform.tfvars` file.

4. Plan the deployment:
   ```bash
   terraform plan
   ```

5. Apply the configuration:
   ```bash
   terraform apply
   ```
   Confirm the prompt with `yes`.

6. After deployment, view output values:
   ```bash
   terraform output
   ```

## Customization
Modify `variables.tf` to adjust parameters such as:
- VM size
- Resource group name
- Location (Azure region)
- Other VM-specific settings

## Clean-Up
To destroy the resources created by this configuration, run:
```bash
terraform destroy
```
Confirm the prompt with `yes`.

## Contributing
Contributions are welcome! Feel free to fork this repository, submit issues, or create pull requests.

## License
This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).

## Contact
For questions or support, please open an issue in this repository.
