# Azure VM Extension Standardisation

## Project Overview

This project implements standardization of Azure Virtual Machine extensions using Azure Policy.

## Problem Statement

Azure Virtual Machines require monitoring and security extensions. When VMs are configured manually, some may have missing or incorrectly configured extensions. This can cause monitoring gaps, security risks, and configuration inconsistencies.

This project uses Azure Policy to detect and manage required VM extensions.

## Technologies Used

- Microsoft Azure
- Azure Virtual Machine
- Azure Monitor Agent (AMA)
- Azure Monitor
- Log Analytics Workspace
- Data Collection Rule (DCR)
- Azure Policy
- Azure CLI
- Linux / Ubuntu

## Implementation

1. Created an Azure Virtual Machine named `TestVM01`.
2. Installed Azure Monitor Agent.
3. Created a Log Analytics Workspace.
4. Created a Data Collection Rule.
5. Connected the VM to the DCR.
6. Verified VM heartbeat data in Log Analytics.
7. Created an Azure Policy to standardize Azure Monitor Agent deployment.
8. Created a security-agent policy to detect missing security configuration.
9. Used Azure Policy compliance and remediation features.

## Architecture

TestVM01 → Azure Monitor Agent → DCR → Log Analytics Workspace

Azure Policy → Checks VM Extension Compliance → Remediation

## Result

The Azure Monitor Agent was successfully installed and monitoring data was verified through Log Analytics.

Azure Policy confirmed the monitoring configuration as compliant and detected the missing security-agent configuration.

## Screenshots

Project screenshots are available in the `screenshots` folder.