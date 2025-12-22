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

# 1.4 Azure Storage Account (Types)

An **Azure Storage Account** provides a unique namespace to store data objects in Azure.

A single storage account can host multiple storage services.

---

## 1.4.1 Blob Storage

Azure Blob Storage is used to store **unstructured data**.

### What it stores

* Text files
* Images
* Videos
* Backups
* Big data files

### Use Cases

* Data lakes
* Media content
* Log storage

### Blob Types

* **Block Blob** – Most common (CSV, JSON, Parquet)
* **Append Blob** – Logs
* **Page Blob** – VHD disks

---

## 1.4.2 File Storage

Azure File Storage provides **file shares** in the cloud.

### Features

* SMB & NFS support
* Mountable like a network drive

### Use Cases

* Lift-and-shift applications
* Shared file systems
* Application configuration storage

---

## 1.4.3 Table Storage

Azure Table Storage is a **NoSQL key-value store**.

### Characteristics

* Schema-less
* Highly scalable
* Low latency

### Use Cases

* Metadata storage
* User profiles
* IoT data

---

## 1.4.4 Queue Storage

Azure Queue Storage is a **message queue service**.

### Features

* Stores large numbers of messages
* Asynchronous communication

### Use Cases

* Decoupling applications
* Background processing
* Event-driven workflows

---

# 1.5 Azure Data Factory (ADF)

Azure Data Factory is a **cloud-based ETL/ELT service** used for data integration.

---

## Introduction to ADF

ADF allows you to:

* Ingest data from multiple sources
* Transform data
* Load data into target systems

It supports:

* Batch processing
* Incremental loads
* Hybrid data integration (on-prem + cloud)

---

## Key Components of ADF

### 🔹 Pipelines

A pipeline is a **logical container** for activities.

Example pipeline:

```
Copy Activity → Data Flow → Sink
```

---

### 🔹 Datasets

Datasets represent the **data structure** used by activities.

Examples:

* Azure Blob Dataset
* Azure SQL Dataset
* ADLS Gen2 Dataset

---

### 🔹 Linked Services

Linked Services define **connection information**.

Examples:

* Azure Blob Storage linked service
* Azure SQL linked service
* Azure Databricks linked service

---

# 1.6 Integration with Azure Services

ADF integrates seamlessly with other Azure services.

---

## 1.6.1 Dataset and Linked Service

### Dataset

* Points to the data
* Defines schema & format

### Linked Service

* Defines connection details
* Uses authentication (Key Vault, Managed Identity)

Example:

```
Linked Service → Dataset → Activity
```

---

## 1.6.2 Integration Runtimes (IR)

Integration Runtime provides the **compute environment** for data movement.

### Types of IR

| IR Type        | Use Case                     |
| -------------- | ---------------------------- |
| Azure IR       | Cloud-to-cloud data movement |
| Self-hosted IR | On-premises integration      |
| Azure-SSIS IR  | Run SSIS packages            |

---

## 1.6.3 Triggers and Monitoring

### Triggers

Triggers define **when pipelines run**.

Types:

* Schedule Trigger
* Tumbling Window Trigger
* Event-based Trigger

---

### Monitoring

ADF provides monitoring for:

* Pipeline runs
* Activity runs
* Trigger status
* Error details

Benefits:

* Retry failed runs
* Debug pipelines
* SLA monitoring

---

## Why These Azure Services Matter

* Centralized data integration
* Scalable storage solutions
* Secure and automated ETL pipelines
* Enterprise-ready cloud architecture

---

# 1.4 Azure Storage Account (Types)

An **Azure Storage Account** provides a unique namespace to store data objects in Azure.

A single storage account can host multiple storage services.

---

## 1.4.1 Blob Storage

Azure Blob Storage is used to store **unstructured data**.

### What it stores

* Text files
* Images
* Videos
* Backups
* Big data files

### Use Cases

* Data lakes
* Media content
* Log storage

### Blob Types

* **Block Blob** – Most common (CSV, JSON, Parquet)
* **Append Blob** – Logs
* **Page Blob** – VHD disks

---

## 1.4.2 File Storage

Azure File Storage provides **file shares** in the cloud.

### Features

* SMB & NFS support
* Mountable like a network drive

### Use Cases

* Lift-and-shift applications
* Shared file systems
* Application configuration storage

---

## 1.4.3 Table Storage

Azure Table Storage is a **NoSQL key-value store**.

### Characteristics

* Schema-less
* Highly scalable
* Low latency

### Use Cases

* Metadata storage
* User profiles
* IoT data

---

## 1.4.4 Queue Storage

Azure Queue Storage is a **message queue service**.

### Features

* Stores large numbers of messages
* Asynchronous communication

### Use Cases

* Decoupling applications
* Background processing
* Event-driven workflows

---

# 1.5 Azure Data Factory (ADF)

Azure Data Factory is a **cloud-based ETL/ELT service** used for data integration.

---

## Introduction to ADF

ADF allows you to:

* Ingest data from multiple sources
* Transform data
* Load data into target systems

It supports:

* Batch processing
* Incremental loads
* Hybrid data integration (on-prem + cloud)

---

## Key Components of ADF

### 🔹 Pipelines

A pipeline is a **logical container** for activities.

Example pipeline:

```
Copy Activity → Data Flow → Sink
```

---

### 🔹 Datasets

Datasets represent the **data structure** used by activities.

Examples:

* Azure Blob Dataset
* Azure SQL Dataset
* ADLS Gen2 Dataset

---

### 🔹 Linked Services

Linked Services define **connection information**.

Examples:

* Azure Blob Storage linked service
* Azure SQL linked service
* Azure Databricks linked service

---

# 1.6 Integration with Azure Services

ADF integrates seamlessly with other Azure services.

---

## 1.6.1 Dataset and Linked Service

### Dataset

* Points to the data
* Defines schema & format

### Linked Service

* Defines connection details
* Uses authentication (Key Vault, Managed Identity)

Example:

```
Linked Service → Dataset → Activity
```

---

## 1.6.2 Integration Runtimes (IR)

Integration Runtime provides the **compute environment** for data movement.

### Types of IR

| IR Type        | Use Case                     |
| -------------- | ---------------------------- |
| Azure IR       | Cloud-to-cloud data movement |
| Self-hosted IR | On-premises integration      |
| Azure-SSIS IR  | Run SSIS packages            |

---

## 1.6.3 Triggers and Monitoring

### Triggers

Triggers define **when pipelines run**.

Types:

* Schedule Trigger
* Tumbling Window Trigger
* Event-based Trigger

---

### Monitoring

ADF provides monitoring for:

* Pipeline runs
* Activity runs
* Trigger status
* Error details

Benefits:

* Retry failed runs
* Debug pipelines
* SLA monitoring

---

## Why These Azure Services Matter

* Centralized data integration
* Scalable storage solutions
* Secure and automated ETL pipelines
* Enterprise-ready cloud architecture

---


