# ALZ-StartSmall
This project provides a small and expandable Azure landing zone delivered as IaC (infrastructure as code) using Bicep.

## Overview

The Azure Landing Zone (ALZ) provided by Big Green IT (BGIT) follows the key design principles of the Azure Cloud Adoption Framework (CAF) to ensure that your Azure environment is secure and scalable. 

Resource groups are used to organize and manage your various Azure resources.  Virtual networks act as the logical data center in the cloud for your workloads and subnets have been configured and are ready for your resources.  Network security groups are used to allow or deny traffic to and from your Azure resources.  The local network gateway is the entry point to your on-prem environment and defines the on-prem subnets that are allowed to access Azure resources. 

The BGIT Azure Landing Zone offering provides customers with an environment that meets Azure’s best practices for Cloud Adoption Framework and gives customers the flexibility to change or customize their environment as needed.  The following resources are automatically deployed as part of your landing zone: 

Resource groups 

Virtual networks 

Subnets 

VPN Gateway 

Network Security Group 

Local Network Gateway 

Resource Tagging 

Azure Policy 

If you need assistance in purchasing this solution or have questions please contact support@biggreenit.com 
## Prerequisites

Azure subscription 

The user deploying the solution must have Owner or Contributor RBAC role assigned 
## User Input

The user will need to provide input for the following: 

Azure Subscription 

Region 
## Identity and RBAC Roles

This project supports the use of Microsoft Entra ID for identity management and RBAC roles can be assigned to govern access to resources. RBAC roles allow the granting of only the required access needed to perform the job. 

https://learn.microsoft.com/en-us/azure/role-based-access-control/best-practices  
## Resource Groups

Resources are organized into resource groups for easier management and governance.  Resource Groups typically contain resources that share the same management or lifecycle so you can easily deploy, update, and delete them as a group. This project creates x number of rgs. 

https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-portal  
## Networking

A traditional hub and spoke network topology is employed allowing for customized builds, enhanced-security, and large-scale networks.  This project includes the creation of virtual networks (VNets), the assignment of IP address space, and the use of Network Security Groups (NSGs), to control access to resources within the VNets. 

IP address space 

VPN Gateway – used for secure hybrid connectivity to Azure resources from on-prem locations over the public internet. 

Local Network Gateway 

https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-best-practices/define-an-azure-network-topology  
## Security

Network security groups are used to control access to resources within the VNets. A network security group contains security rules that allow or deny inbound or outbound access to and from Azure resources.  Additional security measures can be implemented as needed. 

https://learn.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview  

If you need assistance applying security best practices to your Azure resources, please contact sales@biggreenit.com 
## Governance

Governance is one aspect of Azure Management. This project uses Azure Policy as part of the governance strategy to govern, configure, secure, protect, and monitor Azure resources and workloads. Using Azure Policy to enforce resource tagging and regional restrictions meets some of the challenges of managing Azure resources. 

https://learn.microsoft.com/en-us/azure/governance/management-groups/azure-management  

If you need assistance applying additional governance best practices to your Azure resources, please contact sales@biggreenit.com 
## Naming Conventions

Naming conventions and standards take on special importance since there is no way to rename resources in Azure once they are deployed.  The naming conventions follows the best practices of the Cloud Adoption Framework. 
## Authors

- [@octokatherine](https://www.github.com/octokatherine)


## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)

