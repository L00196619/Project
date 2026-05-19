# Week 1

## Background research.

#### Deciding Cloud Service Providers

**Amazon Web Services AWS** was ranked as the top CSP by Geeks for Geeks. AWS has been providing cloud based solutions since 2006. Covering a wide range of services, from AI and databases to maching learning and serverless deployments, AWS offers a total of 175 fully-featured services across database storage, networking, compute, etc. One of the features AWS provides is the free tier which allows users to test and deploy cloud services at a very low cost for a limited time. This feature will be used for this project.

**Azure** was launched a few years after AWS, and remains one of the main competitors in the market. Microsft Azure is ranked second by Geeks for Geeks, after AWS. Azure is wide spread geographically accross 54 regions and operating in 140 countries offering a wide variety of services including AI and machine learning, Databases, Devops, networking etc. Similar to AWS, Azure also offers free trial of 30 days period for new users. Azure will later be implemented and compared against AWS in terms of virtual machine deployment, networking configuration, ease of use and overall functionality.

**Proxmox** is not a cloud service provider itself, but is one of the leading  open-source virtualization platforms used to create and manage virtual machines. Whilst VMware uses its own dedicated VMkernel hypervisor, Proxmox is based on Debian Linux and combines both KVM virtualization and LXC container technologies within the same platform. In this project, Proxmox will be used within a cloud environment.

**Google Cloud** Google Cloud is renowned for its advanced data analytics and AI/ML solutions, and in this project it will be used to compare its virtualization services against both AWS and Microsoft Azure in terms of cost, deployment, performance, and management features. Similar to AWS, Google Cloud offers free tier solution for a limited time of 90 days allowing users to test different features. This feature will be utilized in this project.

## Project planning.

The main objective of this project is to research, deploy, and evaluate cost-effective alternatives to traditional VMware infrastructure using open-source tools and native cloud service providers.

To properly test and evaluate alternatives to vmware, the project will be structrued into three core phases.

### Phase 1 - use native public cloud alternative

In this phase, AWS will be deployed and tested as a cloud-based virtualization platform.

This phase will focus on creating and managing virtual machines within the cloud environment while testing core virtualization features similar to traditional VMware environments.

The following tasks and tests will be carried out:

- Virtual machine deployment and configuration
- Network configuration and connectivity testing
- SSH remote access testing
- Elastic IP (static public IP) configuration
- Additional storage volume creation and attachment
- Snapshot and backup testing
- Machine image (AMI) creation and deployment
- Web server deployment and hosting using Apache
- Testing scalability and cloud management features

The aim of this phase is to evaluate how AWS can provide a low-cost or free alternative to traditional on-premise virtualization platforms. 

### Phase 2 – Use Cloud Hosted Virtualization Platforms

In this phase, Microsoft Azure will be used to test nested virtualization by deploying Proxmox VE inside an Azure virtual machine.

Unlike Phase 1 which focused on native cloud virtualization services, this phase will focus on recreating a more traditional VMware-style virtualization environment within the cloud.

The purpose of this phase is to examine whether a low-cost cloud virtual machine can host a fully virtualized platform capable of running multiple virtual machines inside it. Additionally, "reversibility and Exit Strategy" will be discussed and potential solution will be tested to address vendor lock-in concerns. The project will carry out tests to identify whether a virtual machine created within a cloud-hosted Proxmox VE environment can be successfully exported and migrated back into a traditional VMware environment. This will help evaluate whether organisations can adopt open-source virtualization platforms while still maintaining the ability to return to VMware infrastructure if required.

The following tasks and tests will be carried out:

- Azure virtual machine deployment and networking configuration
- Installation and configuration of Proxmox VE
- Nested virtualization configuration and testing
- Access and testing of the Proxmox graphical management interface
- Creation and management of virtual machines inside Proxmox
- Snapshot and cloning functionality testing
- Storage and virtual disk configuration
- Export testing using OVA/OVF images
- Migration of Proxmox virtual machines into VMware
- Import and compatibility testing within VMware
- Comparison between nested virtualization and traditional VMware environments

The aim of this phase is to evaluate whether nested virtualization using Proxmox inside Azure can provide a practical and low-cost alternative to VMware environment without requiring dedicated physical hardware, whilst demonstrating a possible exit strategy to address vendor lock-in risks.

### Phase 3 - Evaluation of different alternatives to VMWare

In this phase, the cloud platforms and virtualization solutions tested throughout the project will be compared and evaluated based on performance, usability, cost, virtualization features, and overall practicality.

This phase will focus on analysing the results gathered from AWS, Google Cloud native virtualization services, and nested virtualization using Proxmox VE within Azure, and the reversibility and migration testing carried out between Proxmox and VMware environment.

The following areas will be evaluated:

- Ease of virtual machine deployment and configuration
- Network configuration
- Storage management capabilities
- Snapshot and backup functionality
- Virtual machine cloning and Golden Image creation
- Performance and responsiveness of nested virtualization
- Migration compatibility between Proxmox and VMware
- Vendor lock-in considerations and exit strategy effectiveness
- Cost effectiveness and free-tier limitations
- Overall suitability as an alternative to traditional VMware infrastructure
