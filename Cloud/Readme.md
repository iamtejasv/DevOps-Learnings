# Start Your Azure Journey Now!

Begin your Azure journey by watching this playlist.

[Watch the Azure Playlist](https://youtube.com/playlist?list=PLdpzxOOAlwvIcxgCUyBHVOcWs0Krjx9xR&si=m1j2VbRFNEiimxdJ)

# Basics of Cloud Computing

## What is Cloud ?

In simpler terms, imagine the cloud as a vast, virtual space where you can store files, run software, and access various services over the internet. 

It's like having a powerful computer somewhere out there on the web that you can use for tasks without needing to own or physically manage the hardware. This allows users to access data and applications
from anywhere with an internet connection.

## What is Cloud Computing ?

Cloud computing is a technology model that involves the delivery of computing services over the internet. Instead of owning and maintaining physical servers and infrastructure, users can access and use
computing resources, applications, and storage provided by either third-party service providers (public cloud) or their own organization (private cloud) through the internet. These services are hosted
in data centers located around the world.

In essence, cloud computing can involve both third-party providers (public cloud) and an organization's internal resources (private cloud). The distinction lies in whether the computing resources are
shared among multiple customers (public cloud) or dedicated to a single organization (private cloud). The flexibility of cloud computing allows organizations to choose the deployment model that best
aligns with their needs and requirements.

## Public Cloud:

**Who Uses It:** Everyone, like individuals, businesses, and organizations.

**What It's Like:** Imagine a giant, shared computer space on the internet. It's like using apps, storing files, or doing tasks on the internet that anyone can access.

**Example:** Think of Google Drive or Amazon Web Services (AWS).

## Private Cloud:

**Who Uses It:** One specific organization or business.

**What It's Like:** Picture having your own personal, private computer space. It's like a digital clubhouse where only you and your team have access. Others can't just drop in.

**Example:** A company using its own server for all its digital needs.

## Hybrid Cloud:

**Who Uses It:** A mix of everyone, depending on needs.

**What It's Like:** It's like having your private computer space, but sometimes you use the shared internet space too. 

**Example:** A business storing sensitive data in its private space but using the public cloud for extra storage or specific tasks.

### In a Nutshell:

**Public Cloud:** Shared digital space for everyone.

**Private Cloud:** Your own exclusive digital space.

**Hybrid Cloud:** Using both your private space and the shared online space when needed.

# Vocabulary in Cloud Computing

## Virtualization

Virtualization is the process of creating a virtual version of something, such as an operating system, server, storage, or network resources.

## Virtual Machine

A Virtual Machine (VM) is a software-based emulation of a physical computer. It allows running multiple operating systems on a single physical machine.

## API (Application Programming Interface)

API is a set of rules and protocols that allows different software applications to communicate with each other. It defines how software components should interact.

## Regions

Regions in cloud computing refer to geographic locations where cloud providers have data centers. Each region contains multiple data centers.

## Availability Zones

Availability Zones are isolated locations within a region that have their own power, cooling, and networking. They are designed to provide high availability and fault tolerance.

## Scalability

Scalability is the ability of a system to handle an increasing amount of work or its potential to be enlarged to accommodate that growth.

## Elasticity

Elasticity in cloud computing refers to the ability to dynamically scale resources up or down based on demand.

## Agility

Agility is the capability of quickly and easily adapting to changes. In the context of cloud computing, it involves the rapid deployment of resources and applications.

## High Availability

High Availability (HA) ensures that a system or application is operational and accessible for a high percentage of time, typically 99.9% or higher.

## Fault Tolerance

Fault Tolerance is the ability of a system to continue operating without interruption in the presence of hardware or software failures.

## Disaster Recovery

Disaster Recovery involves the planning and processes for restoring and recovering data and systems after a natural or human-induced disaster.

## Load Balancing

Load Balancing is the distribution of network traffic or computing workload across multiple servers to ensure no single server is overwhelmed.

# Compute, Networking and Storage in Cloud Computing

Compute, Networking and Storage are the fundamental pillars of Cloud Computing serving as the backbone for the delivery of various cloud services. They work together seamlessly to provide users with a
robust and scalable computing environment. Let's break down each of these components:

## Compute:

- It refers to the processing power used to run applications, software and workloads in the cloud.
- Cloud providers offer various compute options such as virtual machines (VMs), containers and serverless computing allowing users to choose the right configuration for their specific needs.

## Networking:

- It connects different components of the cloud infrastructure and enables communication between them and involves virtual routers, switches, firewalls, and load balancers to ensure seamless and secure
network traffic flow.

## Storage:

- It provides a secure and reliable space for storing data in the cloud.
- Cloud storage comes in various forms including object storage, block storage and file storage catering to different data types and access needs.

## On-Premises 

On-premises or on prem refers to computing resources such as servers and software that are owned, operated & physically located within an organization's own facilities or data centers. This means the
organization has direct control over the hardware, software & infrastructure used for their IT operations.

## Cloud

Cloud computing involves accessing and utilizing computing resources (such as servers, storage, databases) over the internet, provided by Cloud Service Providers (CSP).

## Azure Budgets

### What are Azure Budgets?

Azure Budgets allow you to set spending limits on your Azure subscriptions, resource groups, or even individual resources. By defining budgets, you gain better control over your costs and can receive
alerts when expenditures approach or exceed specified thresholds.

### Creating and Managing Budgets
1. **Create a Budget:**
   - Use Azure Portal or PowerShell to set up budgets.
   - Specify limits for subscriptions, resource groups, or individual resources.

2. **Manage Budgets:**
   - Modify budgets as needed.
   - Follow best practices for effective budget management.

### Alerts
- Configure alert thresholds to receive notifications when expenditures approach or exceed set limits.

## Cost Management

### What is Cost Management?

Azure Cost Management is a comprehensive service that allows you to monitor, analyze, and optimize your cloud costs. It provides detailed insights into where your money is being spent and helps identify
potential cost-saving opportunities.

### Analysis and Optimization
1. **Cost Analysis:**
   - Review monthly costs and ensure alignment with budgetary limits.
   - Identify abnormal service usage or cost surges.

2. **Azure Budgets Integration:**
   - Set budgets based on cost or usage.
   - Regularly revisit budgets and make necessary adjustments.

3. **Azure Pricing Calculator:**
   - Evaluate pricing for different Azure services.
   - Useful for planning new workloads or expanding existing ones.

4. **Azure Advisor:**
   - Leverage recommendations for cost savings, performance, and availability.
   - Identify underutilized resources and optimize database usage.

### Enabling Cost Management
1. **Access Azure Portal:**
   - Sign in with an enterprise administrator account.

2. **Navigate to Cost Management + Billing:**
   - Click on Billing scopes and select your billing account.

3. **Configure Policies:**
   - Enable Azure Cost Management for authorized users.

Azure Budgets and Cost Management work hand-in-hand to provide a comprehensive approach to controlling and optimizing Azure expenditures. 

[A Comprehensive Guide to Setting Up Your Azure Account and Acquiring Credits](https://dev.to/beingwizard/a-comprehensive-guide-to-setting-up-your-account-and-acquiring-azure-credits-15d2)

# Azure Resource Groups

## What are Azure Resource Groups?

Azure Resource Groups are containers that hold related resources in Azure. These resources can include virtual machines, storage accounts, networking configurations, and more. Resource Groups provide a
way to manage and organize resources efficiently.

## Key Characteristics

1. Resource Groups provide a way to logically organize and manage resources based on your needs. For example, you might create a Resource Group for a specific project, environment (e.g., production,
staging, development), or application.

2. Resources within a Resource Group share a common lifecycle. When you delete a Resource Group, all of its resources are also deleted. This simplifies resource management and cleanup.

3. You can apply access control to a Resource Group, making it easier to manage permissions for a set of resources. This allows you to control who can deploy, manage, or delete resources within a
specific Resource Group.

4. You can assign tags to a Resource Group, making it easier to categorize, filter, and track resources based on specific attributes.

5. Azure resources are often deployed to a Resource Group. When you create a resource, you specify the target Resource Group, and all related resources are provisioned within that group.

## Creating a Resource Group

To create a Resource Group, you typically use the Azure Portal, Azure CLI (Command-Line Interface), PowerShell, or templates (such as Azure Resource Manager templates) to define and deploy the required
resources within the group.
