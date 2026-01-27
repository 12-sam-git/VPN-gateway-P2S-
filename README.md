# VPN-gateway-P2S
create a VPN gateway (p2s):

   🔐 Azure Point-to-Site (P2S) VPN Gateway – Proof of Concept
📌 Overview

This Proof of Concept (POC) demonstrates the implementation of an Azure Point-to-Site (P2S) VPN Gateway to provide secure remote access to Azure resources.
The POC focuses on configuring two authentication methods to understand different security approaches used in real-world enterprise environments.

🎯 Objective

Enable secure remote user connectivity to Azure Virtual Network

Configure and test two P2S authentication mechanisms

Understand the purpose of each Azure networking and security component

Gain hands-on experience with Azure VPN Gateway configuration

🏗️ Architecture Summary

Users connect from external networks (home/office)

Traffic flows securely over the internet

Azure VPN Gateway acts as the entry point

Authentication is handled using:

Certificates

Microsoft Entra ID (Azure Active Directory)

🔐 Authentication Methods Implemented
1️⃣ Certificate-Based Authentication

Uses Root and Client certificates

Suitable for labs, POCs, and small environments

Does not depend on identity provider availability

2️⃣ Microsoft Entra ID Authentication

Uses Azure AD identities

Supports MFA and Conditional Access

Recommended for enterprise and production environments

🛠️ Azure Services Used

Azure Resource Group

Azure Virtual Network (VNet)

Gateway Subnet

Azure VPN Gateway

Point-to-Site VPN Configuration

Microsoft Entra ID (Azure Active Directory)

Public IP Address

🧩 Step-by-Step Implementation (High Level)

Created a Resource Group to logically group VPN resources

Created a Virtual Network to provide private address space

Created a mandatory GatewaySubnet for VPN Gateway

Deployed a Route-based Azure VPN Gateway

Configured Point-to-Site VPN settings

Implemented Certificate-based authentication

Implemented Microsoft Entra ID authentication

Tested VPN connectivity using both methods

Detailed step-by-step explanation with “What we did” and “Why we did it” is available in the documentation file.

✅ Validation & Testing

Successfully connected using certificate-based authentication

Successfully authenticated using Microsoft Entra ID credentials

Verified IP allocation from P2S address pool

Confirmed access to Azure VNet resources

🔒 Security Considerations

VPN traffic is encrypted using SSL/TLS

Certificate authentication ensures device trust

Entra ID authentication enables identity-based access control

User access restricted using Azure AD assignments

📚 Key Learnings

Difference between Point-to-Site and Site-to-Site VPN

Importance of GatewaySubnet in Azure networking

Certificate-based vs Identity-based authentication

Real-world use cases of Azure VPN Gateway

Secure remote access design in Azure

👩‍💻 Target Audience

Azure Freshers

Cloud & Network Engineers

Students preparing for Azure interviews

Professionals learning Azure networking security

📌 Author

Sameeksha Y S
Azure | Cloud | Networking | Security

📎 Repository Usage

This repository is created for:

Learning and practice

Interview discussion

Portfolio showcase

Internal team knowledge sharing
