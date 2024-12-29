# Azure Setup with Terraform

This project provides a guide for setting up and managing Azure resources using Terraform. Follow the steps below to configure and deploy your infrastructure.

---

## How It Works

### 1. Prepare Your Environment
- Ensure you have an active Azure subscription.
- Use [Azure Cloud Shell](https://docs.microsoft.com/en-us/azure/cloud-shell/features) for an easier setup.
  _If you're not using Azure Cloud Shell, additional configurations are required._

### 2. Download the Azure Setup Script
Run the following command to download the script:

```bash
wget https://github.com/hashicorp/packer/blob/master/contrib/azure-setup.sh
```

### 3. Make the Script Executable
Set execution permissions for the script:

```bash
chmod +x azure-setup.sh
```
### 4. Run the Setup Script
For non-Azure Cloud Shell environments, run:

```bash
./azure-setup.sh setup
```
Follow the instructions carefully and save the output for future use

### 5. Configure Your Setup
Copy the sample configuration file:

```bash
cp setup.sh.sample setup.sh
```

### 6. Apply the Configuration
Source the configuration to load environment variables:

```bash
. ./setup.sh
```


### 7. Deploy Resources with Terraform
Run the following command to provision your Azure infrastructure:

```bash
terraform apply
```


## Features
- Ease of Use: Simplified deployment using Terraform and Azure Cloud Shell.
- Customizable Setup: Modify the configuration file to suit your project needs.
- Streamlined Workflow: Automate infrastructure deployment and management effortlessly.



## Requirements
- An active Azure account
- Azure CLI (if not using Azure Cloud Shell)
- Terraform installed locally or accessible via Azure Cloud Shell

## Getting Started
- Use the setup script to configure your Azure environment.
- Update setup.sh to include your Azure credentials and preferences.
- Execute Terraform commands to manage your resources.

## Contributions and Feedback
Contributions are welcome! If you encounter issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License
This project is licensed under the [MIT License](https://github.com/korhanh/Terraform-Azure/blob/main/README.md).

Feel free to use, modify, and distribute this project according to the terms specified in the license.

## Credits
Created and maintained by korhanh.








