# Azure Storage Account IP Rule Management Script

## Overview

This script contains a Bash script that automates the process of adding multiple IP addresses to the network rules of an Azure Storage account. This is particularly useful for scenarios where you want to restrict access to your storage account to specific IP addresses, such as those used by Azure Front Door or Azure CDN. These IPs are based on the IPs of service tag AzureFrontDoor.Backend.

## Problem Statement

When using Azure Storage accounts, you may want to enhance security by limiting access to only certain IP addresses. This is especially important when integrating with services like Azure Front Door or Azure CDN, which require specific IP addresses to be whitelisted in the storage account's network rules. Manually adding each IP address can be time-consuming and error-prone, especially when dealing with a large number of addresses.

## Solution

The provided script automates the process of adding a predefined list of IP addresses to the network rules of an Azure Storage account. By running this script, you can quickly and efficiently configure your storage account to allow access from the specified IPs.

## Prerequisites

- **Azure CLI**: Ensure that you have the Azure CLI installed on your machine. You can download it from [here](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli).
- **Azure Account**: You must have an active Azure account and the necessary permissions to modify the storage account's network rules.
- **Bash Environment**: The script is written in Bash, so you will need a Bash-compatible terminal (Linux, macOS, or Windows Subsystem for Linux).

## Usage

1. **Clone the Repository**: Clone this repository to your local machine.

   ```bash
   git clone https://github.com/davisdre/azure_scripts.git
   cd bash/add_storage_ip_rules
   ```

2. **Run the Script**: Execute the script to add the IP addresses to your storage account's network rules.

    ```bash
    ./add_storage_ip_rules.sh
    ```