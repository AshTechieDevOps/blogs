# AWS Storage Core

## On-Premises Storage versus AWS Cloud Storage

For many organizations, moving to the cloud starts with an assessment of their existing on-premises storage infrastructure. Organizations that take the time to identify where and how their data is stored, have a head start in moving their existing workloads to the AWS Cloud. As you explore the available AWS Storage services, you can compare the storage service offerings to your on-premises storage infrastructure. 

In this lesson, you will learn to compare existing on-premises storage with AWS Storage service options and effectively assess your existing storage infrastructure. You will learn to identify patterns for diverse application and workload needs.

## Why organizations move to the cloud

Moving storage workloads to the cloud has been one of the main ways chief information officers (CIOs) can address their top strategic priorities:

## Increase Organization Agility

###  On-premises storage agility challenges

-   Resources are required to make changes to on-premises storage infrastructure. Resources include time, personnel, data center space and infrastructure, and fixed and variable costs. Capacity planning, resource planning, and budgeting are required before you can implement changes. As a result, the time to implement changes can be delayed from weeks to months or even years. 

-   Even after approval, it can take weeks or months to order, receive, and install new systems or additional capacity for existing ones. Many organizations offer provision storage capacity to deal with implementation and budgeting delays. The unused capacity consumes space and costly resources while waiting to be used.

-   On-premises storage infrastructure lacks the option to quickly reduce or change environments as your organization's needs change. After your storage is in place, it usually remains in place regardless of its use. Being able to re-allocate storage capacity from one storage silo or system to another silo or system is seldom possible. Most storage systems do not have the compatibility required for cross-system integration.

### Storage agility in AWS

#### AWS Storage services provide solutions to address the on-premises storage agility challenges. When using AWS Storage services, you can quickly change existing storage services or implement new ones.

-   AWS manages the required resources for you. You do not need to allocate time, implementation and management personnel, data center space and infrastructure, or use fixed and variable costs to change your storage infrastructure. You manage how you use the storage services that you provision.

-   You have access to virtually unlimited storage capacity when you need it. You can add storage capacity on demand without over-provisioning capacity.

-   You can reduce capacity or discontinue use of a storage service at any time. Your storage service use is not restrained by physical system limitations. 

-   With AWS services, you can move data between different storage silos or systems as needed. After copying your data to a different service, you can delete the source service, or delete the data from the service to save money. 

## Accelerate ablility to innovate

-   To innovate, you must be able to develop and test new workflows on demand. For example, a test and development environment must be flexible to try different designs and workflows and then make changes as needed. You must often scale the development environment for testing. Conversely, you must also be able to abandon an environment after testing is completed, or abandon any temporary environments when no longer needed.  

-   To innovate with on-premises storage systems, you need to purchase new systems or use unused capacity on existing systems. Purchasing new systems takes time and resources. Using existing systems can present challenges with available capacity or having the correct type of resource required.

-   With on-premises storage systems, often the data is contained in separate storage systems that create silos that are disconnected from each other. The separation makes it difficult to access the systems to perform analytics or use machine learning across systems.

-   With AWS Storage, you can start development on one service and experiment using different services to meet your workflow's requirements. You can increase or reduce capacity as needed for your development and testing environment. Using AWS Storage services provides you a flexible environment for innovation.

## Strengthen Security 

### On-premises storage and network infrastructure are often not uniformly secured from external or internal access. Security concerns include:

-   Physical security access to storage systems

-   Consistent encryption for data at rest and data in transit

-   Appropriate user, group, and role access controls

-   External network attacks or system hacking

### Organizations can improve their security posture as they gain insights by removing data silos and improving encryption controls. With AWS, you inherit all of the controls, tools, best practices, and certifications designed for even the most security-conscious organizations. 

### Cloud providers secure the cloud infrastructure and separate the infrastructure from the customer applications. The benefit is you no longer need to be concerned about infrastructure security.

## Reduce Costs

-   With cloud storage, you do not have to purchase hardware, provision storage, or provide capital for "someday" scenarios. You can add or remove capacity on demand, quickly change performance and retention characteristics, and pay only for storage that you actually use. You can move less frequently accessed data automatically to lower-cost tiers in accordance with auditable rules. This flexibility drives economies of scale. 

## Operational expense versus capital investment

-   A benefit of moving to the cloud is shifting expenses from fixed or variable costs to ongoing costs. Instead of paying for system and software expenses up front and then realizing the expenses over time, cloud services are charged as a monthly expense. This reduces budgeting and ordering fulfillment cycles and realizes the expenses when they occur.

### Cloud storage is typically purchased from a third-party cloud vendor that owns and operates data storage capacity and delivers it over the internet in a pay-as-you-go model. These cloud storage vendors manage capacity, security, and durability to make data accessible to your applications all around the world.

### Applications access cloud storage through traditional storage protocols or directly through an API. Many vendors offer complementary services designed to help collect, manage, secure, and analyze data at massive scale.



### Cloud storage is a reliable, scalable, and secure place for your data. AWS offers a complete range of services for you to store, access, govern, and analyze your data to reduce costs, increase agility, and accelerate innovation. You don’t have to perform a one-to-one replacement of your on-premises storage (also known as lift and shift). Instead, you can re-platform or re-architect your storage to optimize cost, manageability, and performance based on your applications needs.

### Comparison of storage use: What you pay for

<img width="646" alt="AWSCore1" src="https://user-images.githubusercontent.com/110538923/196687260-3745b101-8035-4e5b-8214-7dbf1bb911cd.PNG">

#### When you acquire new on-premises storage systems or additional storage capacity for your existing systems, you purchase the total raw capacity for the system. You then need to host the system in your data center and maintain the total capacity. 

#### With AWS Storage, you can add new storage services or expand existing services on demand to meet your requirements. AWS hosts and maintains the underlying systems in their data centers. 

#### You can compare the options using the general example between on-premises storage capacity and AWS Storage services capacity. As you explore the remainder of this course, more details are provided for each of the AWS Storage services.

### On-premises storage capacity

<img width="269" alt="AWSCore2" src="https://user-images.githubusercontent.com/110538923/196688290-d28631c3-9c69-4bc9-bf26-3a2b3a1f18bd.PNG">

#### When you purchase on-premises storage, you work backwards from the capacity you need to store your data and provide for growth and performance overhead. You purchase the total raw capacity to meet your requirements and anticipated capacity growth. Because of certain variables, you are required to make forward-looking assumptions to estimate your requirements.

#### In the example, several broad assumptions are applied to perform the calculations for how much storage to acquire. The calculations applied in real life are different for every on-premises system. The calculations can vary significantly based on the manufacturer. The important takeaways from this example is to consider the aspects that reduce the usable capacity and that you pay for the raw capacity.

#### Please read the following to learn about a specific category:-

##### Raw Capacity

-   Using the on-premises storage example, you purchase 1 petabyte (PB) of raw storage capacity. This is what you pay for and what is needed to calculate the operating costs and data center requirements. 

-   The net usable capacity will vary by manufacturer and by individual system.

##### Formatted Capacity

##### Every storage system's capacity is reduced from hardware failure protection overhead, drive formatting, and operating system overhead. The amount varies based on how this is implemented on the system. In the example, this reduces the capacity by 20 percent to 800 TB.

-   Hardware failure protection overhead – Typically known as hardware or software redundant array of independent disks (RAID). The primary purpose is to protect the data if hardware or a drive fails by creating checksum protection for the data. Depending on the protection level, this can amount 15%–50% overhead. For example, RAID 1, drive mirroring, creates mirrored drive pairs (50 percent overhead). RAID 6 uses two drives worth of space to store checksums (15%–25% overhead). You can apply other protection schemes. However, hardware failure protection is part of every system. 

-   Formatting and operating system overhead – Drive capacity is typically represented in unformatted capacity. When formatted by the operating system, the drive size is reduced 1%–5%. The operating system is then added to the system, which further reduces the available capacity.

##### Allocated Capacity

##### The available capacity is further reduced when you account for data protection services, such as snapshots, and add space for performance overhead. In the example, this reduces the capacity by an additional 200 TB–600 TB of allocated capacity. 

-   Snapshots can consume more space than your actual data. Snapshots help you protect against data corruption and accidental deletion.

-   To operate efficiently and increase performance, systems require additional space for operation overhead, especially for write operations. 

##### Actual Data Capacity

##### You estimate that you need at least 400 terabytes (TB) of actual data capacity. The remaining 200 TB above your actual 400 TB of data is allocated for data and snapshot growth.

### Capacity options for AWS Storage services

<img width="264" alt="AWSCore3" src="https://user-images.githubusercontent.com/110538923/196701338-6f746acd-2e30-4f2b-9e01-303700658951.PNG">

-   Billing increments are as small as per second of use. In addition to capacity billing, additional service charges might be incurred for service use. The different billing components are discussed later in this course.

-   Some services, such as Amazon Simple Storage Service (Amazon S3), are based on the amount of storage capacity that you consume. You pay only for the storage capacity that you use.

-   Other services, such as Amazon Elastic Block Store (Amazon EBS), are based on the amount of the capacity that you allocate. For example, when you create a block store of 20 GB, you are allocating 20 GB of capacity for use. With allocated capacity, you pay for the allocated amount of space and not the amount of data you have stored.

-   With Amazon Elastic File System (Amazon EFS), you have the option to use the default setting of consumed storage or provisioned storage. Select the option to meet your use case and application performance requirements.

### Capacity overhead in AWS Cloud

#### You still have to provision more space to accommodate the following elements in AWS.

-   Formatting
-   File system
-   Hardware failure protection
-   Data protection
-   Operating system overhead

##### However, AWS absorbs and manages the extra capacity requirements. AWS considers the systems and maintenance overhead when determining pricing for the storage service. With AWS Storage, you can focus on your business while AWS takes care of systems and maintenance. 

## Primary storage types

### Whether on premises or in a cloud environment, you have three primary types of storage: block, file, and object. Different storage hardware manufacturers and cloud service providers implement these storage types differently. However, the fundamentals for each storage type are basically the same, regardless of where the storage type is located, who manufactures the hardware, or who provides the service. The specific features and functionality differ based on how the manufacturer or service provider implements the storage.


<img width="643" alt="AWSCore4" src="https://user-images.githubusercontent.com/110538923/196708658-8b91966b-b938-4a28-a669-1cca8408dd2d.PNG">

### To get started, you should have a fundamental understanding of the primary storage types and the differences between them. 

#### Block Storage Overview:-

-   Block storage is raw storage in which the hardware storage device or drive is a disk or volume that is formatted and attached to the compute system for use. The storage is formatted into predefined continuous segments on the storage device. These segments are called blocks. The blocks are the basic fixed storage units used to store data on the device.
-   Storage devices can be hard disk drives (HDDs), solid state drives (SSDs), or newer types of storage devices, such as Non-Volatile Memory Express (NVMe). In addition to individual storage devices, you can deploy block storage on storage area network (SAN) systems.
-   The storage device is used by the operating system or an application that has the capabilities to manage block storage directly. For cases in which the application manages the block storage, the application often shares management with an operating system.

#### File Storage Overview:-

-   File storage is built on top of block storage, typically serving as a file share or file server. File storage is created using an operating system that formats and manages the reading and writing of data to the block storage devices. The name file storage comes from the primary use of storing data as files typically in a directory tree hierarchy.
-   The two most common storage protocols for file storage are Server Message Block (SMB) and Network File System (NFS). You can use the network protocols to communicate with remote computers and servers. You can also use server resources or share, open, and edit files.
-   The operating system manages the storage protocol and the operation of the file system. The file system can be Windows Server, Linux, or a specialized operating system used on network attached storage (NAS) devices or clustered NAS systems.

#### Object Storage Overview:-

-   Object storage is also built on top of block storage. Object storage is created using an operating system that formats and manages the reading and writing of data to the block storage devices. The name object storage comes from the primary use of storing the data within a binary object. Unlike file storage, object storage does not differentiate between types of data. The type of data or the file type becomes part of the data's metadata.
-   An object is made up of a larger set of blocks organized by using a predetermined size. For example, one object storage system uses binary object sizes of 128 megabytes (MB). Smaller files or data are stored at a binary level within the object. Larger data files are stored by spreading the data across multiple objects.
-   Object storage is recognized for its inherent availability of the file objects. Some systems support file versioning, file tracking, and file retention.













