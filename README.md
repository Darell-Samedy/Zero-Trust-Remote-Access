# Zero-Trust-Remote-Access

# Overview

Zero Trust Remote Access Platform

This repository showcases my Zero Trust Remote Access project, designed and implemented in Microsoft Azure. The project demonstrates modern cloud security principles, including identity-based access, network segmentation, and secure remote connectivity, without exposing resources to the public internet. It’s a practical example of my skills in cloud security, networking, and enterprise-level architecture, designed to demonstrate hands-on experience for IT, cybersecurity, and cloud-focused roles.

# Features

- Zero Trust Architecture – Implements least-privilege access principles.
- Secure Remote Access – Uses Azure Bastion to connect to internal VMs without public IP exposure.
- Network Segmentation – Hub and application VNets for secure isolation.
- Access Control – Identity-based authentication and authorization.
- Monitoring & Logging – Integration with Azure Monitor and Log Analytics for visibility and auditing. 

Tools & Technologies
- Cloud Platform: Microsoft Azure
- Networking: VNets, Subnets, NSGs, VNet Peering
- Security: Azure Bastion, Azure Firewall, Zero Trust Principles
- Monitoring: Azure Monitor, Log Analytics
- OS: Windows Server, Ubuntu Linux
- Protocols: SSH, RDP, HTTPS

# Diagram of Project:

![image_alt](https://github.com/Darell-Samedy/Zero-Trust-Remote-Access/blob/main/screenshots/ZERO%20TRUST%20DIAGRAM%20HOMELAB.png?raw=true)

# Implementation Steps ( All Screenshots/Configurations located within the screenshots folder )

Step 1: Set up Virtual Networks (VNets)
  - Created a Hub VNet and an App VNet in Azure.
  - Configured /24 subnets for network isolation.
  - Ensured proper peering between VNets for controlled traffic flow.

Step 2: Deploy Azure Bastion
  - Deployed Azure Bastion in the Hub VNet.
  - Enabled secure RDP/SSH access to VMs without exposing them to the public internet.
  - Tested Bastion connectivity from your local machine.

Step 3: Configure Access Policies
  - Implemented least-privilege rules to restrict who can access VMs.
  - Configured network security groups (NSGs) to enforce traffic rules.
  - Verified access restrictions by testing unauthorized connection attempts.

Step 4: Deploy Virtual Machines
  - Deployed Windows Server and Ubuntu Linux VMs in the App VNet.
  - Configured firewall rules inside VMs and ensured Bastion access only.
  - Installed minimal services for testing connectivity and monitoring.

Step 5: Enable Monitoring & Logging
  - Connected VNets and VMs to Azure Log Analytics.
  - Configured logging for network rules, application rules, and NSG flows.
  - Verified logs to confirm network activity and successful access events.

Step 6: Test Zero Trust Access
  - Attempted access from devices outside the network.
  - Verified that only authenticated users via Bastion could connect.
  - Confirmed that traffic from unauthorized sources was blocked.

# Learning Outcomes
- Applied Zero Trust security principles in a cloud environment.
- Gained hands-on experience with Azure networking and security services.
- Implemented secure remote access for internal applications.
- Learned how to monitor, troubleshoot, and log network activity in Azure.

# Future Improvements/Configurations
- Integrate Azure Sentinel for advanced monitoring and alerts. (Configured but found difficulty)
- Privileged Identity Management (PIM)
    - Force “approval + time limit” for admin roles
    - Shows real-world enterprise control
 - PowerShell Automation Scripts

# About Me

I’m Darell Samedy, a technology enthusiast specializing in cloud security, networking, and IT infrastructure. This project reflects my hands-on approach to implementing modern security practices in real-world cloud environments.

GitHub: https://github.com/DarellSamedy

LinkedIn: https://linkedin.com/in/darellsamedy
