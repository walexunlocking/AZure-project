#  Summary Report

## 1. Selected Azure Region
* **Chosen Region:** Canada Central 
* **Reasoning:** Selected based on geographical proximity to minimize network latency and ensure compliance with local data residency preferences. Choosing a region with robust Availability Zone support also ensures higher infrastructure resilience.

## 2. Shared Responsibility Model Breakdown
The division of responsibilities depends entirely on the type of resource deployed during this lab.

### Scenario A: If you deployed a Virtual Machine (IaaS)
Infrastructure as a Service (IaaS) shifts the physical infrastructure management to Microsoft, but leaves the operating system and software stack under user control.

* **Microsoft's Responsibility:** Physical security of the datacenter, hardware hosts, physical networking, and cooling infrastructure.
* **My (The User's) Responsibility:** Managing, patching, and securing the guest Operating System (OS), configuring network security groups (firewall rules), managing user access permissions, and protecting the data stored inside the VM.

### Scenario B: If you deployed a Storage Account (PaaS)
Platform as a Service (PaaS) abstracts away the underlying operating system, leaving the user responsible only for the data and access management.

* **Microsoft's Responsibility:** Operating system patching, physical hardware, network infrastructure, storage replication, and baseline platform security.
* **My (The User's) Responsibility:** Configuring data access keys, setting up Shared Access Signatures (SAS), managing identity permissions via RBAC, and data classification/governance.
