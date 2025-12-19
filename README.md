# ADF

# 1. Key Features and Services

## 1.1 Global Data Centers

Azure operates a global network of **data centers** distributed across multiple regions worldwide.

### Key Points

* Regions are geographically isolated
* Each region contains one or more data centers
* Supports data residency and compliance requirements

### Benefits

* Low latency access
* High availability
* Disaster recovery
* Global scalability

Examples:

* Central India
* East US
* West Europe

---

## 1.2 Azure Subscription and Resource Groups

### What is an Azure Subscription?

An Azure Subscription is a **billing and access boundary** in Azure.

A subscription:

* Tracks usage and billing
* Controls access via RBAC
* Contains multiple resource groups

---

### 1.2.1 Creating Azure Subscription

Ways to create a subscription:

* Azure Portal
* Azure Free Account
* Enterprise Agreement (EA)
* Pay-As-You-Go

Basic steps:

1. Sign in to Azure Portal
2. Go to **Subscriptions**
3. Click **Add**
4. Choose subscription type
5. Complete payment setup

---

### 1.2.2 Managing Resources in Resource Groups

#### Resource Groups

* Logical containers for Azure resources
* Resources share lifecycle

Example:

```
Resource Group: prod-rg
 ├── Virtual Machine
 ├── Storage Account
 ├── Virtual Network
```

Management Operations:

* Create / Delete
* Move resources between RGs
* Apply tags for cost management
* Set RBAC permissions

---

## 1.3 Azure Workspace and UI

Azure provides multiple interfaces to manage resources.

---

### 1.3.1 Navigating the Azure Portal

Azure Portal is a **web-based GUI** for managing Azure resources.

Key sections:

* Home
* Dashboard
* All services
* Resource groups
* Subscriptions

Capabilities:

* Create resources
* Monitor performance
* Configure security

---

### 1.3.2 Overview of Dashboard and Resource Management

#### Dashboard

* Customizable view
* Pin frequently used resources
* Monitor metrics & alerts

#### Resource Management

* Create / update / delete resources
* Monitor usage
* Apply policies

---

### 1.3.3 Azure CLI and PowerShell

Azure supports **command-line management** for automation and scripting.

| Tool       | Platform                 |
| ---------- | ------------------------ |
| Azure CLI  | Cross-platform           |
| PowerShell | Windows & Cross-platform |

---

### 1.3.4 Command-Line Interface Options for Azure

#### Azure CLI

* Uses `az` commands
* Works on Windows, Linux, macOS

Example:

```bash
az login
az group create --name myRG --location centralindia
```

---

### 1.3.5 Scripting with PowerShell

Azure PowerShell uses cmdlets.

Example:

```powershell
Connect-AzAccount
New-AzResourceGroup -Name myRG -Location "Central India"
```

### Why Use PowerShell?

* Automation
* Repeatable deployments
* Infrastructure as Code support

---

## Why These Azure Features Matter

* Simplified cloud management
* Centralized billing and access control
* Multiple management interfaces
* Enterprise-ready governance

---

