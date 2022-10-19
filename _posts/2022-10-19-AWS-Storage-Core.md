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

## Introduction to the AWS Storage Portfolio

### The AWS Storage portfolio consists of the core storage services and other closely associated services. You select the services you need based on what you are trying to accomplish.

### With AWS Storage, you can quickly provision the storage that is best suited for your application or use case. You can use a combination of storage services to meet your requirements without the need to provision, host, and maintain separate systems. 

### Because you pay for only the resources that you use, you can provision storage to do the following:

-   Test new applications
-   Test use cases
-   Try different storage services for your existing ones

#### When you are finished, you can delete the storage resource. 

#### All AWS Storage services include configurable security services. Your data is private by default. You must allow access to your data from the public, from other AWS services, or from other AWS accounts. Securing your data is a top-level concern.

### AWS Storage services

<img width="492" alt="AWSCore5" src="https://user-images.githubusercontent.com/110538923/196711448-248a99d1-890f-4924-bbae-a0bcd5b249d3.PNG">

### The AWS core storage services are block, file, and object. Each offers its own advantages based on the workload and has its own use cases.

### Block Storage:- 

-   Some enterprise applications, such as databases or ERP systems, often require dedicated, low-latency storage for each host. This is analogous to direct-attached storage (DAS) or a Storage Area Network (SAN). Block-based cloud storage solutions are provisioned with each virtual server and offer the ultra low latency required for high-performance workloads.
-   Amazon Elastic Block Store (Amazon EBS) is used to attach to Amazon Elastic Compute Cloud (Amazon EC2) instances. As with on-premises block storage, the operating system or application manages storage access. Amazon EBS is offered in different options to meet your organization's use case requirements.

### File Storage:-

#### Some applications need to access shared files and require a file system. This type of storage is often supported with a Network Attached Storage (NAS) server. File storage solutions are ideal for use cases such as large content repositories, development environments, media stores, or user home directories.

#### AWS currently offers file storage using five different services. These services are divided into two categories, Amazon's own cloud native file storage and the Amazon FSx file storage offerings. FSx stands for "file system X". These offering implement managed files storage using the commonly available file systems for on-premises solutions. 

#### You also have the option to create self-managed files shares using Amazon EC2 instances with attached Amazon EBS volumes. 

#### Each file service offers different feature sets to meet your requirements.

-   Amazon Elastic File System (Amazon EFS) is a multi-Availability Zone file storage service that uses NFS access protocol. 
-   Amazon FSx for Lustre is built using the Lustre file system and is designed for high performance computing (HPC) and machine learning (ML) workloads. FSx for Lustre uses the Lustre client's POSIX-compliant access protocol.
-   Amazon FSx for Windows File Server is built using Windows File Server. The access protocol is Server Message Block (SMB) and designed for your Microsoft applications and Windows workloads.
-   Amazon FSx for NetApp ONTAP is built using the NetApp ONTAP operating system and is designed to provide both NetApp block and file storage. The access protocols are iSCSI for block storage, NFS and SMB for file storage.
-   Amazon FSx for OpenZFS  fully managed shared file storage built on the OpenZFS file system. With Amazon FSx for OpenZFS, you can migrate your on-premises OpenZFS storage to AWS with minimal effort. You can use the same access protocols now in the AWS Cloud.

### Object Storage:-

#### Applications developed in the cloud often take advantage of object storage's vast scalability and metadata characteristics. Object storage solutions are ideal for building modern applications from the beginning that require scale and flexibility. The solution is also ideal for importing existing data stores for analytics, backup, or archive.

#### Amazon Simple Storage Service (Amazon S3) is object storage in the AWS Cloud. Amazon S3 is offered with different storage classes or tiers to match your price, access, and availability requirements. Amazon S3 Glacier, for example, is used for archival storage at a lower cost per gigabyte (GB).

#### AWS uses Amazon S3 as cost effective storage to store snapshots and backups of data stored in other core storage services such as Amazon EBS and Amazon EFS.

### Core AWS Storage services 

<img width="649" alt="AWSCore6" src="https://user-images.githubusercontent.com/110538923/196713543-bd5f8753-9411-4544-88e9-ba45fe02cab5.PNG">

### Edge and hybrid cloud storage services

<img width="646" alt="AWSCore7" src="https://user-images.githubusercontent.com/110538923/196713748-c3d520b3-7f4b-4440-9a63-92f4b2667586.PNG">

### AWS offers services that are designed to provide edge and hybrid cloud solutions. Edge compute and storage solutions for remote or disconnected locations and hybrid solutions to connect your on-premises infrastructure to storage services in the AWS Cloud.

### Edge - Local Compute and Storage

#### With edge location compute and storage services, you can use compute resources and storage services even when disconnected from the AWS Cloud. They also provide a data transfer platform to copy your data in to and out from the AWS Cloud. You can transfer your data by shipping the devices to AWS for import or use the device as a remote data synchronization client. 

#### Edge location devices include the AWS Snow Family of products: AWS Snowball devices, AWS Snowcone devices, and AWS Snowmobile service.

#### AWS Snowball is an edge computing, data migration, and edge storage device. You can use these devices for the following:-

-   Data collection
-   Machine learning and processing
-   Storage in environments with intermittent connectivity or in remote disconnected locations

#### Snowball Edge comes in two options: Storage Optimized for the highest storage capacity and Compute Optimized for more available vCPUs with a lower storage capacity.

#### AWS Snowcone is the smallest member of the AWS Snow Family of edge computing, edge storage, and data transfer devices, weighing in at 4.5 pounds (2.1 kg). Snowcone is ruggedized, secure, and purpose-built for use outside of a traditional data center.

#### AWS Snowmobile is an exabyte-scale data transfer service used to move large amounts of data to AWS. You can transfer up to 100 PB per Snowmobile, a 45-foot long ruggedized shipping container, pulled by a semitrailer truck. Snowmobile makes it easy to move massive volumes of data to the cloud, including video libraries, image repositories, or even a complete data center migration.

### Hybrid - On-Premises Cloud Storage

#### On-premises cloud storage is provided as part of an AWS Outposts implementation and includes Amazon EBS and Amazon S3 storage services. 

#### AWS Outposts is a fully managed service that offers the same AWS infrastructure, AWS services, APIs, and tools to virtually any data center, colocation space, or on-premises facility. These capabilities provide a consistent hybrid experience. AWS Outposts is ideal for the following:-

-   Workloads that require low latency access to on-premises systems, local data processing, and data residency
-   Migration of applications with local system interdependencies

#### AWS compute, storage, database, and other services run locally on Outposts. You can access the full range of AWS services available in the Region to build, manage, and scale your on-premises applications using familiar AWS services and tools.

### Hybrid - On-Premises Gateways

#### AWS Storage Gateway connects on-premises users and applications using a software appliance with cloud-based storage. It provides integration between an organization’s on-premises IT environment and the AWS storage infrastructure. You can use Storage Gateway to simplify storage management and reduce costs for key hybrid cloud storage use cases. 

#### Use cases include the following:-

-   Moving backups to the cloud
-   Using on-premises file shares backed by cloud storage
-   Providing low-latency access to data in AWS for on-premises applications. Local caching reduces network latency for both read and write activities.

### Storage Gateway offers four different types of gateways: Amazon S3 File Gateway, Amazon FSx File Gateway, Volume Gateway, and Tape Gateway.

-   Amazon S3 File Gateway provides a seamless way to connect to the cloud to store application data files and backup images as durable objects in Amazon S3. Amazon S3 File Gateway offers SMB or NFS-based access to data in Amazon S3 with local caching. 
-   Amazon FSx File Gateway optimizes on-premises access to fully managed, highly reliable file shares in Amazon FSx for Windows File Server. Customers with unstructured or file data, whether from SMB-based group shares or business applications, might require on-premises access to meet low-latency requirements.
-   Volume Gateway presents cloud-backed iSCSI block storage volumes to your on-premises applications. Volume Gateway stores and manages on-premises data in Amazon S3 on your behalf and operates in cache mode or stored mode. 
-   Tape Gateway is used to replace physical tapes on premises with virtual tapes in AWS without changing existing backup workflows. Tape Gateway supports all leading backup applications and caches virtual tapes on premises for low-latency data access.

## Edge and hybrid cloud storage services

<img width="646" alt="AWSCore8" src="https://user-images.githubusercontent.com/110538923/196734766-e177df3a-636f-406a-8983-0f41b12a297b.PNG">

## Data transfer and migration services

<img width="651" alt="AWSCore9" src="https://user-images.githubusercontent.com/110538923/196735104-53fcc4f4-753a-4d4a-8a99-6e9204fb5fd9.PNG">

### Data transfer services are designed to copy or transfer your on-premises data to and from the core AWS Storage services in the AWS Cloud.

### File Transfer Services

### The AWS Transfer Family provides fully managed support for file transfers directly into and out of Amazon S3 or Amazon EFS. AWS Transfer Family includes support for Secure File Transfer Protocol (SFTP), File Transfer Protocol over SSL (FTPS), and File Transfer Protocol (FTP). 

### The AWS Transfer Family helps you to migrate your file transfer workflows to AWS by doing the following so that nothing changes for you or your applications:-

-   Integrating with the specified authentication system
-   Providing DNS routing with Amazon Route 53

### Data Synchronization and Online Transfer Services

### AWS DataSync is an online data transfer service that simplifies, automates, and accelerates moving data between on-premises storage systems and AWS Storage services and between AWS Storage services. You can use DataSync for the following operations:-

-   Migrate active datasets to AWS
-   Archive data to free up on-premises storage capacity
-   Replicate data to AWS for business continuity
-   Transfer data to the cloud for analysis and processing

### DataSync can copy data between the following resources or services:-

-   Network File System (NFS) shares
-   SMB shares
-   Self-managed object storage
-   AWS Snowcone
-   Amazon S3 buckets
-   Amazon EFS file systems
-   Amazon FSx for Windows File Server file systems

### Offline Data Transfer and Migration Services

### Offline data transfers are performed using AWS Snow Family devices. The AWS Snow Family helps customers who need to run operations in austere, non-datacenter environments, and in locations where there’s lack of consistent network connectivity.

### The Snow Family, comprised of AWS Snowcone, AWS Snowball, and AWS Snowmobile, offers several physical devices and capacity points, most with built-in computing capabilities. These services help to physically transport up to exabytes of data into and out of AWS.

### AWS owns and manages Snow Family devices. The devices integrate with AWS security, monitoring, storage management, and computing capabilities.

### Migration Services

### AWS Application Migration Service (AWS MGN), which includes CloudEndure Migration, is a highly automated lift-and-shift (rehost) solution. AWS MGN simplifies, expedites, and reduces the cost of migrating applications to the AWS Cloud, AWS GovCloud (US), and AWS Outposts.

### You can use AWS MGN or CloudEndure Migration by itself to quickly lift-and-shift physical, virtual, or cloud servers without compatibility issues, performance impact, or long cutover windows. AWS MGN continuously replicates your source servers to your AWS account. When you’re ready to migrate, it automatically converts and launches your servers on AWS.

## AWS data transfer and migration services

<img width="654" alt="AWSCore10" src="https://user-images.githubusercontent.com/110538923/196737936-15986056-c517-4e67-b588-a672ed398a12.PNG">

## Data protection services

<img width="652" alt="AWSCore11" src="https://user-images.githubusercontent.com/110538923/196738262-8a408624-8319-4853-96cd-0caf51b2cbe7.PNG">

### Data protection services provide optional services to meet your data redundancy and disaster requirement needs. Some services are standalone service options and some are integrated into the core storage services. 

## Backup and Archive

### Using AWS Backup, you can centralize and automate data protection across AWS services. AWS Backup offers a cost-effective, fully managed, policy-based service that further simplifies data protection at scale. AWS Backup also helps you support your regulatory compliance or business policies for data protection.

### When you combine AWS Organizations with AWS Backup, you can deploy data protection policies centrally. Centrally deploy policies to configure, manage, and govern your backup activity across your company’s AWS accounts and resources. Resources include the following:-

-   Amazon EC2 instances
-   Amazon EBS volumes
-   Amazon RDS databases (including Amazon Aurora clusters)
-   Amazon DynamoDB tables
-   Amazon Neptune databases
-   Amazon DocumentDB (with MongoDB compatibility) databases
-   Amazon EFS
-   Amazon FSx for Lustre
-   Amazon FSx for Windows File Server
-   AWS Storage Gateway volumes
-   Amazon Simple Storage Service (Amazon S3) buckets
-   VMware workloads on premises and in VMware CloudTM on AWS

### Snapshots

### Native snapshot services are built into most core services. Snapshots create backup copies of your data. Snapshots are stored in a protected part of Amazon S3 as part of the managed service. Storing snapshots on Amazon S3 protects your data with 99.999999999 percent (11 9s) of durability and provides you Regional access and availability.

### Snapshots are incremental copies of the data, which means that only the data that has changed after your most recent snapshot is saved in the next incremental snapshot. Incremental snapshots reduce the time required to create the snapshot. These incremental snapshots save on storage costs by not duplicating previously saved data. Each snapshot contains all of the information for that point in time that is needed to restore your data.

### Replication

### Storage replication is an available built-in feature for some of the core storage services. How replication is implemented varies for each service. Replication increases availability and protects your data by creating additional copies. Replication can be between Availability Zones within an AWS Region or between AWS Regions.

### Disaster Recovery Services

### CloudEndure Disaster Recovery service provides a cost-effective disaster recovery option for your on-premises servers and applications. 

### CloudEndure Disaster Recovery continuously replicates your machines into a low-cost staging area in your target AWS account and preferred Region. Replication also includes operating system, system state configuration, databases, applications, and files. In the case of a disaster, you can instruct CloudEndure Disaster Recovery to automatically launch thousands of your machines in their fully provisioned state in minutes. 

### CloudEndure Disaster Recovery minimizes downtime and data loss by providing fast, reliable recovery of physical, virtual, and cloud-based servers into AWS Cloud, including AWS Regions, AWS GovCloud (US), and AWS Outposts.

## Data protection services

<img width="647" alt="AWSCore12" src="https://user-images.githubusercontent.com/110538923/196741577-6eb0d9ce-79a9-4226-b72b-bcd3f3075388.PNG">


## AWS Storage services portfolio

### Now that you have a high-level understanding of what each of the services is, you will learn more about each of the services in more detail later in this series of courses. A view of the standalone services that comprise the AWS Storage portfolio is provided for your review.  

<img width="648" alt="AWSCore13" src="https://user-images.githubusercontent.com/110538923/196742076-70db48e1-b779-44bf-a3e1-dfc3918dfb73.PNG">


## Identifying the Right Storage Solution in the Cloud

### The optimal storage solution for a system varies based on the following:-

-   Type of access method (block, file, or object)
-   Patterns of access (random or sequential)
-   Required throughput-

-   How often and how quickly do you need to access your data? AWS offers storage options and pricing tiers for frequently accessed, less frequently accessed, and infrequently accessed data.
-   Does your data store require high IOPS or throughput? AWS provides categories of storage that are optimized for performance and throughput. Understanding IOPS and throughput requirements will help you provision the right amount of storage and avoid overpaying.
-   What storage access protocols are required? Pre-existing applications are often developed based on specific operating systems. The operating system can affect the access protocol. For example, Linux-based applications that require file system access usually require NFS. Windows-based applications require SMB as the protocol. 
-   
-   Frequency of access (online, offline, archival)
-   Frequency of update (WORM, dynamic)
-   Availability and durability constraints

### The AWS Well-Architected systems use multiple storage solutions and enable different features to improve performance and use resources efficiently. For additional information about AWS Well-Architected systems.

## Storage characteristics and requirements

### You must understand the different characteristics of your application or workflow that are required to select the services that best fit your workload. Example characteristics are shareable, file size, cache size, access patterns, latency, throughput, and persistence of data. Those characteristics can lead you toward the best storage solution, such as block storage, file storage, or object storage.

### To optimize storage, the first step is to understand the performance profile for each of your workloads. Conduct a performance analysis to measure input/output operations per second (IOPS), throughput, and other variables. Define your storage performance requirements. Identify your workload’s most important storage performance metrics. Use those metrics to set boundaries. Implement improvement strategies as part of a data-driven approach, using benchmarking or load testing. Use this data to identify where your storage solution is or can be constrained. Examine storage and configuration options to improve the solution. 

### AWS storage services are optimized for different storage scenarios. No single data storage option is ideal for all workloads. When evaluating your storage requirements, consider data storage options for each workload separately.

### Determine the expected growth rate for your workload and choose a storage solution that will meet those rates. Object and file storage solutions, such as Amazon S3 and Amazon Elastic File System, enable unlimited storage.

## Questions to help determine storage requirements

### The following questions help you to segment data within each of your workloads and determine your storage requirements:-

-   How often and how quickly do you need to access your data? AWS offers storage options and pricing tiers for frequently accessed, less frequently accessed, and infrequently accessed data.
-   Does your data store require high IOPS or throughput? AWS provides categories of storage that are optimized for performance and throughput. Understanding IOPS and throughput requirements will help you provision the right amount of storage and avoid overpaying.
-   What storage access protocols are required? Pre-existing applications are often developed based on specific operating systems. The operating system can affect the access protocol. For example, Linux-based applications that require file system access usually require NFS. Windows-based applications require SMB as the protocol. 
-   How critical (durable) is your data? Critical or regulated data needs to be retained at almost any expense and tends to be stored for a long time.
-   How sensitive is your data? Highly sensitive data must be protected from accidental and malicious changes, not only data loss or corruption. Durability, cost, and security are equally important to consider.
-   How large is your dataset? Knowing the total size of the dataset helps in estimating storage capacity and cost.
-   How transient is your data? Transient data is short-lived and typically does not require high durability. (Note: Durability refers to average annual expected data loss.) Clickstream and Twitter data are good examples of transient data.
-   How much are you prepared to pay to store the data? Setting a budget for data storage will inform your decisions about storage options.

## Evaluate available configuration options

### Evaluate the various characteristics and configuration options and how they relate to storage. Understand where and how to use the following elements to optimize storage space and performance for your workload:-

-   Provisioned IOPS
-   Solid state drives (SSD)
-   Hard disk drives (HDD)
-   Object storage
-   Archival storage
-   Ephemeral (temporary) storage 

## Determine storage characteristics

### When you evaluate a storage solution, determine the available storage characteristics, such as the following:-

-   Ability to share the storage
-   Ideal file size and maximum file size
-   Storage cache size
-   Average or expected latency
-   Maximum throughput
-   Maximum IOPS
-   Persistence of data

#### Then match your requirements to the AWS service that best fits your needs.

## Make decisions based on access patterns and metrics

### Choose storage systems based on your workload's access patterns. Configure them by determining how the workload accesses data. You can sometimes increase storage efficiency or increase a performance metric by choosing a different storage type. Configure the storage options you choose to match your data access patterns. 

-   Optimize your storage usage and access patterns – Choose storage systems based on your workload's access patterns and the characteristics of the available storage options. Determine the best place to store data so that you can meet your requirements while reducing overhead. Use performance optimizations and access patterns when configuring and interacting with data based on the characteristics of your storage (for example, striping volumes or partitioning data).
-   Select appropriate metrics for storage options – Ensure that you select the appropriate storage metrics for the workload. Each storage option offers various metrics to track how your workload performs over time. Make sure that you are measuring against any storage metrics indicating peak performance and trends. For storage systems that are fixed sized, such as Amazon Elastic Block Store (Amazon EBS) or Amazon FSx, ensure that you are monitoring the amount of storage used against the overall storage size. Create automation when possible to increase the storage size when reaching a threshold.
-   Monitor metrics – Amazon CloudWatch can collect metrics across the resources in your architecture. You can also collect and publish custom metrics to surface business metrics or derived metrics. Use CloudWatch or third-party solutions to set alarms that indicate when thresholds are breached.

### For additional information, see Storage Architecture Selection in the AWS Well-Architected Framework.

## Block Storage: Amazon EBS

### The AWS block storage portfolio consists of two types of block storage services: Amazon Elastic Compute Cloud (Amazon EC2) instance storage and Amazon Elastic Block Store (Amazon EBS). Amazon EBS also includes an integrated snapshot service. Amazon EBS is the primary block storage service. 

### Amazon FSx for NetApp ONTAP also offers block storage services over an iSCSI access protocol. These block services use NetApp's application programming interface (API) calls and management interface. For customer's seeking an integrated NetApp approach, block storage is available as part of the Amazon FSx service.

## Amazon EC2 instance store

### An instance store provides temporary (ephemeral) block-level storage for your instance. This storage is located on disks that are physically attached to the host computer where the compute instance is. Instance stores resemble Amazon EBS storage in initial configuration options. However, their architecture most closely resembles direct attached disk drives. An instance store provides submillisecond latencies between the EC2 instance and the storage.

### Only specific Amazon EC2 instance types support instance stores. The available storage type is directly associated to the EC2 instance type. An instance store consists of one or more instance store volumes exposed as block devices. The size of an instance store and the number of devices available vary by instance type. 

### Instance store is ideal for the following use cases:-

-   Temporary storage of information that changes frequently, such as buffers, caches, scratch data, and other temporary content
-   Data that is replicated across a fleet of instances, such as a load-balanced pool of web servers

### Instances stores are not recommended for most block storage workloads.

### As ephemeral storage, instance stores are not replicated or spread across multiple devices to improve durability and availability. An instance store is nonpersistent and is terminated when the associated EC2 instance is terminated.

## Instance store lifetime

### The data in an instance store persists only during the lifetime of its associated EC2 instance. If an instance reboots (intentionally or unintentionally), data in the instance store persists. However, data in the instance store is lost under any of the following circumstances:-

-   The underlying disk drive fails
-   The instance stops
-   The instance hibernates
-   The instance terminates

### Therefore, do not rely on an instance store for valuable, long-term data. Instead, use more durable data storage, such as Amazon EBS, for your block storage requirements.

## Amazon EBS overview

### Amazon EBS is an easy-to-use, high performance, block storage service. It is designed for use with Amazon EC2 compute instances for both throughput and transaction-intensive workloads at any scale. 

### AWS recommends Amazon EBS for data that must be quickly accessible and requires long-term persistence. EBS volumes are well suited for use as the primary storage for file systems, databases, or any applications that require fine granular updates and access to raw, unformatted, block-level storage. Amazon EBS is well suited to both database-style applications that rely on random reads and writes and to throughput-intensive applications that perform long, sequential reads and writes.

### EBS volumes behave like raw, unformatted block devices. You can mount these block devices as EBS volumes on your EC2 instances. EBS volumes that are attached to an EC2 instance are exposed as raw block storage volumes that persist independently from the life of the instance. You can create a file system on top of these volumes or use them in any way you would use a block device (such as a hard drive). You can dynamically change the configuration of a volume attached to an EC2 instance, unlike traditional disk drives that come in fixed sizes.

### You can choose from different EBS volume types to balance optimal price and performance. You can achieve single-digit millisecond latency for high-performance database workloads, such as SAP HANA, or gigabyte-per-second throughput for large, sequential workloads such as Apache Hadoop. You can change EBS volume types, tune performance, or increase volume size without disrupting your critical applications. Amazon EBS provides you cost-effective block storage when you need it.

### Designed for mission-critical systems, EBS volumes are replicated within an AWS Availability Zone and can scale to store petabytes of data. Also, you can use EBS snapshots with automated lifecycle policies to back up your volumes in Amazon Simple Storage Service (Amazon S3). You can do this  while ensuring geographic protection of your data and business continuity.

### With Amazon EBS, you pay only for the storage and resources that you provision.

## Amazon EBS features

### Single Availability Zone

### You create an EBS volume in a specific Availability Zone, and then attach it to an EC2 instance in that same Availability Zone. The proximity of your Amazon EBS volume to your Amazon EC2 instance provides low latency and high-performance block storage for your workload.

### To make a volume available outside of the Availability Zone, you can create a snapshot and restore that snapshot to a new volume anywhere in the same AWS Region. You can also copy snapshots to other AWS Regions and then restore them to new volumes there. Snapshots make it easier to use multiple AWS Regions for geographical expansion, data center migration, and disaster recovery.

### Persistent

### Amazon EBS volumes are durable and persistent by default. Your EBS volume survives even if your EC2 instance is terminated. Your data is preserved for your future use and persists until you decide to delete it. Root EBS volumes created with an EC2 instance are terminated with the instance by default. However, you can modify the volume to be persistent.

### EBS volumes are managed independently from the Amazon EC2 instances to which they are attached. You can detach an existing EBS volume from an EC2 instance and reattach it to a different EC2 instance. This provides you the ability to change EC2 instance types to meet your performance requirements and optimize your Amazon EC2 costs. 

### Volume Types

### Amazon EBS provides multiple volume types that you can use to optimize storage performance and cost for a broad range of applications. These volume types are divided into two major categories: SSD-backed storage for transactional workloads, such as databases, virtual desktops, and boot volumes, and HDD-backed storage for throughput-intensive workloads, such as MapReduce and log processing.

### SSD-based volumes include two levels to meet your application requirements: General Purpose SSD volumes and Provisioned IOPS SSD volumes:-

-   General Purpose SSD volumes (gp3 and gp2) balance price and performance for transactional applications, including virtual desktops, test and development environments, and interactive gaming applications.
-   Provisioned IOPS SSD volumes are the highest performance EBS volumes (io2 and io1) for your most demanding transactional applications, including SAP HANA, Microsoft SQL Server, and IBM DB2.

### HDD-based volumes include Throughput Optimized HDD (st1) for frequently accessed, throughput-intensive workloads and the lowest cost Cold HDD (sc1) for less frequently accessed data.

### You can choose the volume type that best meets your application and use case requirements. You can change from one volume type to another.

### Elastic Volumes

### Using the Elastic Volumes feature, you can adapt your volumes as the needs of your applications change. Use this feature to increase capacity, tune performance, and change the type of any new or existing current generation volume dynamically, with no downtime or performance impact. You can easily right-size your deployment and adapt to performance changes.

### The Elastic Volumes feature makes it easier to adapt your resources to changing application demands. You can make modifications in the future as your business needs change.

### High Availability and High Durability

### EBS volumes are designed to be highly available, reliable, and durable at no additional charge to you. EBS volume data is replicated across multiple servers in an Availability Zone to prevent the loss of data from the failure of any single component. 

### Amazon EBS volumes are designed to provide 99.8–99.9 percent durability with an annual failure rate (AFR) of 0.1–0.2 percent. Amazon EBS also supports a snapshot feature, which is a good way to take point-in-time backups of your data. 

### Amazon EBS offers a higher durability io2 volume that is designed to provide 99.999 percent durability with an AFR of 0.001 percent. In this case, failure refers to a complete or partial loss of the volume. This makes io2 ideal for business-critical applications, such as SAP HANA, Oracle, Microsoft SQL Server, and IBM DB2, that will benefit from higher uptime. 

### Data Encryption

### You can create your EBS volumes as encrypted volumes to meet a wide range of data-at-rest encryption requirements for regulated/audited data and applications. When you create an encrypted EBS volume and attach it to a supported instance type, data stored at rest on the volume, disk I/O, and snapshots that were created from the volume are all encrypted. The encryption occurs on the servers that host EC2 instances, providing encryption of data in transit from EC2 instances to Amazon EBS storage.

### Native Snapshot Support

### You can create point-in-time snapshots of EBS volumes, which are persisted to Amazon S3. Snapshots protect data for long-term durability. You can use snapshots to restore your data to new volumes, expand the size of a volume, or move volumes across Availability Zones. The same snapshot can be used to instantiate as many volumes as you want. You can copy these snapshots across AWS Regions. You pay for only the storage capacity consumed for your snapshot data.

### Snapshots let you geographically protect your data and achieve business continuity. You can use Amazon Data Lifecycle Manager (Amazon DLM) to automate snapshot management without any additional overhead or cost.

### AWS Backup Support

### AWS Backup supports backing up your EBS volumes. With AWS Backup, you can centralize and automate data protection across multiple Amazon EBS volumes. AWS Backup offers a cost-effective, fully managed, policy-based service that further simplifies data protection at scale. 

### AWS Backup also helps you support your regulatory compliance obligations and meet your business continuity goals.

### Performance Monitoring

### Performance metrics, such as bandwidth, throughput, latency, and average queue length, are available through the AWS Management Console. Amazon CloudWatch provides these metrics so that you can monitor the performance of your volumes. You can make sure that you are providing enough performance for your applications and paying only for resources you need.

## Amazon EBS use cases

### The functionality and available performance options make Amazon EBS a good storage option for many workloads and use cases. In this section, you will learn about the most common use cases for Amazon EBS storage, including enterprise applications, relational databases, nonrelational (NoSQL) databases, big data analytics, and file systems and media workflows.

## Below are the common Amazon EBS use cases:-

<img width="268" alt="AWSCore14" src="https://user-images.githubusercontent.com/110538923/196760784-a09fe6ff-1775-461a-ab60-324d2d13b453.PNG">

<img width="275" alt="AWSCore15" src="https://user-images.githubusercontent.com/110538923/196761560-c1162292-e758-4619-9086-8f4b659eca62.PNG">

<img width="270" alt="AWSCore16" src="https://user-images.githubusercontent.com/110538923/196762133-8ab3f6ee-bc25-4c99-916b-51072fa5d9ca.PNG">

<img width="275" alt="AWSCore17" src="https://user-images.githubusercontent.com/110538923/196762468-892627ad-331a-4efd-8e2b-a78784200c7c.PNG">

<img width="251" alt="AWSCore18" src="https://user-images.githubusercontent.com/110538923/196762747-8c604ade-d6d9-4087-a039-a75df36dcf2c.PNG">

## Lift and shift on-premises applications using Amazon EBS

## Most organizations have on-premises applications burdened with high capital expenses, complex management, scalability challenges, and hardware that needs to be replaced every 3–5 years.

## Maintaining existing on-premises infrastructure results in increased operational burden. This maintenance drains IT budgets for organizations that are already budget and resource strapped. With these on-premises challenges, IT organizations want to move to the cloud and away from the traditional, costly lifecycle of buying, managing, and replacing on-premises hardware, software, services, and networking.

## Most cloud migrations happen in phases to minimize risk and shorten time to production. The most common approach is to lift and shift an application and its data with as few changes as possible to similar services running in the cloud. This provides the fastest time to production. After the application is on AWS, you can modernize and re-architect application elements to take advantage of the cloud services and optimizations that provide the most significant benefits.

## AWS offers lift-and-shift migration by providing automated tools such as AWS Application Migration Service (AWS MGN) and AWS Server Migration Service (AWS SMS).

## Pricing

## With Amazon EBS, you pay only for what you use. Pricing for EBS volumes is based on the volume type, provisioned volume size, and the provisioned IOPS and throughput performance. EBS volume pricing varies based on the Availability Zone where it resides. The pricing for Amazon EBS snapshots is based on the actual amount of storage space that you use.

## For additional information about EBS volume and EBS snapshot pricing, see Amazon Elastic Block Store Pricing page on the AWS website.

## File Storage Overview

## AWS currently offers three different managed file storage services to meet your application, workflow, and use-case requirements. In addition, you can use Amazon EBS to create self-managed file systems.

<img width="639" alt="AWSCore19" src="https://user-images.githubusercontent.com/110538923/196768874-4d07086a-4c36-4463-a792-40580197af87.PNG">

## For running file systems workflows on AWS, you can select from Amazon Elastic File System (Amazon EFS), Amazon FSx for Lustre, Amazon FSx for NetApp ONTAP, Amazon FSx for OpenZFS, Amazon FSx for Windows File Server, or you can build your own high-performance network file system designed for your workload protocol.

### Amazon EFS is a scalable, elastic, cloud-native file system for Linux. Amazon EFS supports the Network File System (NFS) protocol.

### Amazon FSx for Lustre is an AWS fully managed parallel file system built on Lustre for high performance computing (HPC) workloads. FSx for Lustre supports the Lustre POSIX-compliant protocol.

### Amazon FSx for NetApp ONTAP is the NetApp ONTAP operating system implemented as a fully managed service. FSx for NetApp ONTAP support iSCSI for block storage, NFS protocol for POSIX-compliant access, and SMB protocol for Windows-compatible access.

### Amazon FSx for OpenZFS is an AWS fully managed implementation of the Open Zettabyte File System (ZFS). FSx for OpenZFS supports NFS and SMB protocols for a wide range of application implementations. 

### Note: SMB protocol access is not support at initial service launch.

### Amazon FSx for Windows File Server is an AWS fully managed file system for Windows environments. FSx for Windows File Server supports the Server Message Block (SMB) protocol.

### Using Amazon EC2 and Amazon EBS, you can quickly create your own high-performance block storage for building your own network file system, including the following protocols and systems:-

-   SMB
-   NFS
-   Extents File System (XFS)
-   General Parallel File System (GPFS)
-   Zettabyte File System (ZFS)
-   Other customer files systems

### You can choose the file system that you need to optimize your applications or workflows. You can bring your media workflows and use their native file system running on EC2 instances and store your data on EBS volumes.

<img width="618" alt="AWSCore20" src="https://user-images.githubusercontent.com/110538923/196770214-39149009-2eff-40c0-b4fb-a0069bfbb2ea.PNG">

## File Storage: Amazon EFS

## Amazon Elastic File System (Amazon EFS) provides a simple, serverless, elastic file system for use with AWS cloud services and on-premises resources. It is designed to scale on demand to petabytes without disrupting applications, growing and shrinking automatically. You can add and remove files, eliminating the need to provision and manage capacity to accommodate growth.

## Amazon EFS overview

## Amazon EFS has a simple web services interface where you can create and configure file systems quickly and easily. The service manages all the file storage infrastructure for you, meaning that you can avoid the complexity of deploying, patching, and maintaining complex file system configurations.

## Amazon EFS file systems can grow to petabyte scale, drive high levels of throughput, and allow massively parallel access from compute instances to your data.

## Amazon EFS supports the Network File System version 4 (NFSv4.1 and NFSv4.0) protocol. The applications and tools that you use today work seamlessly with Amazon EFS. Multiple compute modules can access an Amazon EFS file system at the same time. These modules include include Amazon EC2, AWS Lambda, Amazon Elastic Container Service (Amazon ECS), and Amazon Elastic Kubernetes Service (Amazon EKS). Accessing compute services provides a common data source for workloads and applications running on more than one compute instance or container.

## With Amazon EFS, you pay only for the storage used by your file system, with no minimum fee or setup cost. Amazon EFS offers a range of storage classes designed for different use cases. These include:-

-   Standard storage classes – EFS Standard and EFS Standard–Infrequent Access (Standard–IA), which offer multiple Availability Zones (Multi-AZ) resilience and the highest levels of durability and availability.
-   One Zone storage classes – EFS One Zone and EFS One Zone–Infrequent Access (EFS One Zone–IA), which offer additional savings by choosing to save data in a single-Availability Zone (Single-AZ).

## Amazon EFS offers the following:-

-   Simple interface through the AWS Management Console, the AWS Command Line Interface (AWS CLI), or the Amazon EFS API.
-   File system access semantics, such as strong data consistency and file locking. You can use Amazon EFS to control access to your file systems through Portable Operating System Interface (POSIX) permissions. 
-   Supports authentication, authorization, and encryption capabilities to help you meet your security and compliance requirements. 

## Provides the throughput, input/output operations per second (IOPS), and low latency needed for a broad range of workloads. With Amazon EFS, you can choose from two performance modes and two throughput modes:-

-   The default General Purpose performance mode is ideal for latency-sensitive use cases, such as web serving environments, content management systems, home directories, and general file serving. File systems in the Max I/O mode can scale to higher levels of aggregate throughput and IOPS. The tradeoff is slightly higher latencies for file metadata operations.
-   Using the default Bursting Throughput mode, throughput scales as your file system grows. Using Provisioned Throughput mode, you can specify the throughput of your file system independent of the amount of data stored.

## Amazon EFS features

### Fully Managed

### Amazon EFS is a fully managed service providing NFS shared file system storage for Linux workloads. Amazon EFS makes it simple to create and configure file systems. You don't have to worry about managing file servers or storage, updating hardware, configuring software, or performing backups. In seconds, you can create a fully managed file system by using the AWS Management Console, the AWS CLI, or an AWS SDK.

### Highly availability and durability

### Amazon EFS is designed to be highly available and is designed for 99.999999999 percent (11 9s) durability. By default, every Amazon EFS file system object (directory, file, and link) is redundantly stored across multiple Availability Zones for file systems using Standard storage classes. 

### A file system using Standard storage classes can be accessed concurrently from all Availability Zones in the Region where it is located. This means that you can architect your application to fail over from one Availability Zone to other Availability Zones in the Region to ensure the highest level of application availability. Mount targets are designed to be highly available within an Availability Zone for all Amazon EFS storage classes.

### If you select Amazon EFS One Zone storage class, your data is redundantly stored within a Single-AZ. Amazon EFS is designed to sustain concurrent device failures by quickly detecting and repairing any lost redundancy. 

### Storage Classes and Lifecycle Management

## Amazon EFS offers Standard and One Zone storage classes for both frequently accessed and infrequently accessed files. The Amazon EFS Standard-IA and Amazon EFS One Zone-IA storage classes are cost-optimized for files accessed less frequently. 

## You can start saving on your storage costs by enabling EFS lifecycle management for your file system and choosing an age-off policy of 7,14, 30, 60, or 90 days. With EFS lifecycle management policies enabled, files automatically move from Amazon EFS Standard storage to EFS Standard-IA storage, or from Amazon EFS One Zone storage to EFS One Zone-IA storage. Lifecycle management reduces storage costs by up to 92 percent.

## Using the industry accepted estimate that 20 percent of data is actively used and 80 percent is infrequently accessed, you can store your files on Amazon EFS at a cost-effective reduced price. 

## Amazon EFS transparently serves files from both frequently accessed and infrequent access storage classes from a common file system namespace. Therefore, you don't have to worry about which of your files are actively used and which are infrequently accessed.

## Security and Compliance

## You can control network access to your file systems by using Amazon Virtual Private Cloud (Amazon VPC) security group rules. You can also control application access to your file systems by using AWS Identity and Access Management (IAM) policies and Amazon EFS access points. Amazon EFS satisfies many eligibility and compliance requirements to help you meet your regulatory needs.

## Scalable Performance

## Amazon EFS is designed to provide the throughput, IOPS, and low latency needed for a broad range of workloads. Throughput and IOPS scale as a file system grows. Throughput and IOPScan burst to higher throughput levels for short periods of time to support the unpredictable performance needs of file workloads. For the most demanding workloads, Amazon EFS can support performance over 10 GB/sec and over 500,000 IOPS.

## Shared File Systems with NFS v4.0 and v4.1 Support

## Amazon EFS provides secure access for thousands of connections for Amazon EC2 instances, AWS container and serverless compute services, and on-premises servers. The service uses a traditional file permissions model, file locking, and hierarchical directory structure using the NFSv4 protocol. Amazon EC2 instances can access your file system across Availability Zones and Regions. By contrast, on-premises servers can access file systems using AWS Direct Connect or AWS Virtual Private Network (AWS VPN).

## Performance Modes

## Amazon EFS is designed to provide the throughput, IOPS, and low latency needed for a broad range of workloads and offers two performance modes: General Purpose and Max I/O:-

-   General Purpose provides the lowest latency per file system operation and can achieve this for random or sequential I/O patterns. 
-   Max I/O can scale to higher levels of aggregate throughput and operations per second. It is ideal for highly parallelized applications that can scale out to thousands of Amazon EC2 instances. Max I/O performance mode is available only on Amazon EFS file systems using Standard storage classes.

## Throughput Modes

## Amazon EFS offers two throughput modes: Bursting and Provisioned. The throughput mode helps determine the overall throughput a file system can achieve:-

-   With Bursting Throughput, the throughput scales with the size of the file system. Throughput bursts dynamically as needed to support the spiky nature of many file-based workloads.
-   Provisioned Throughput is designed to support applications that require higher dedicated throughput than the default Bursting mode. You can configure the throughput independently of the amount of data stored on the file system.

## Elastic and Scalable

## With Amazon EFS, storage capacity is elastic, growing and shrinking automatically as you add and remove files. With elastic capacity, no provisioning is necessary. You are billed for only what you use. 

## Amazon EFS is designed to be highly scalable both in storage capacity and throughput performance. It can grow to petabyte scale and allows massively parallel access from Amazon EC2 instances to your data. With Amazon EFS, throughput and IOPS scale as a file system grows, and file operations are delivered with consistent, low latencies.

## Encryption

## Amazon EFS offers encryption for data at rest and in transit, providing a comprehensive encryption solution to secure both your stored data and data in transit. 

## Data at rest is transparently encrypted by using encryption keys managed by the AWS Key Management Service (AWS KMS). This management removes the need to build and maintain a key management infrastructure. 

## Encryption of data in transit uses open-standard Transport Layer Security (TLS) to secure network traffic without having to modify your applications. 

## Containers and Serverless File Storage

## Amazon EFS integrates with AWS containers and serverless compute services that require shared storage for latency-sensitive and IOPS-heavy workloads at any scale.

## Amazon EFS provides applications running on Amazon ECS, Amazon EKS, AWS Fargate, and AWS Lambda, access to shared file systems for stateful workloads.

## Data Transfer and Backup

-   AWS DataSync – AWS DataSync is a managed data transfer service. Use this service to move data between on-premises storage and Amazon EFS. 
-   AWS Backup – AWS Backup is a fully managed backup service. Use this service to manage and automate backups of your Amazon EFS file systems centrally. AWS Backup reduces the need for costly, custom solutions and manual processes. The service goes beyond backing up Amazon EFS and centralizes the backup of data across other AWS services in the cloud and on premises. 
-   AWS Transfer Family – AWS Transfer Family provides fully managed support for file transfers directly into and out of Amazon EFS. AWS Transfer Family supports Secure File Transfer Protocol (SFTP), File Transfer Protocol over SSL (FTPS), and File Transfer Protocol (FTP).

## Amazon EFS use cases

## The functionality and available performance options make Amazon EFS well suited to support a broad spectrum of use cases, from home directories to business-critical applications.

## Expand each section to to learn more about common Amazon EFS use cases. Select the + symbol next to each category.

## Containers and Serverless Persistent File Storage

## Using Amazon EFS, you can persist data and state from your containers and serverless functions. This capability provides cloud-native shared files that are high performance, fully managed, elastic, highly available, and scalable. 

## These same attributes are shared by Amazon ECS, Amazon EKS, AWS Fargate, and AWS Lambda. Consequently, developers don’t need to design for these features. The services are ready for modern application development with data persistence. 

## Amazon EFS allows data to be persisted separately from compute, and enables applications to have availability and durability across Availability Zones. Amazon EFS provides a shared persistence layer that allows stateful applications to elastically scale up and down, such as for the following:-

-   DevOps
-   Web serving
-   Web content systems
-   Media processing
-   Machine learning
-   Analytics
-   Search index
-   Stateful microservices applications

## Move to Managed File Systems

## Amazon EFS provides the scalability, elasticity, availability, and durability to be the file store for enterprise applications and applications delivered as a service. Its standard file system interface, file system permissions, and directory hierarchy make it easy to do the following:-

-   Migrate enterprise applications from on premises to the AWS Cloud
-   Build new applications 

## Move your business critical, Linux-based applications to managed file systems with Amazon EFS, while lowering your total cost of ownership (TCO).

## Analytics and Machine Learning

## Amazon EFS provides the ease of use, scalability, performance, and consistency needed for machine learning and big data analytics workloads. Data scientists can use Amazon EFS to create personalized environments. These environments can include home directories storing notebook files, training data, and model artifacts. Amazon SageMaker integrates with Amazon EFS for training jobs, allowing data scientists to iterate quickly.

## Web Serving and Content Management

## Amazon EFS provides a durable, high-throughput file system for content management systems and web serving applications that store and serve information for a range of applications. Examples of applications include websites, online publications, and archives. Amazon EFS adheres to the expected file system directory structure, file naming conventions, and permissions that web developers are accustomed to. Therefore, it can easily integrate with web applications.

## Application Testing and Development

## Amazon EFS provides your development environments a common storage repository in which you can share code and other files in a secure and organized way. You can provision, duplicate, scale, or archive your test, development, and production environments with a few steps. Consequently, your organization can be more agile and responsive to customer needs.

## Media and Entertainment

## Media workflows often depend on shared storage to manipulate large files. Example workflows include video editing, studio production, broadcast processing, sound design, and rendering. 

## Amazon EFS provides a strong data consistency model with high throughput and shared file access. This consistency model cuts the time it takes to perform these jobs and consolidate multiple local file repositories into a single location for all users.

## Database Backups

## Amazon EFS presents a standard file system that you can mount with NFSv4 from database servers. This provides an ideal platform to create portable database backups using native application tools or enterprise backup applications. Your company might want to take advantage of the flexibility of storing database backups in the cloud for temporary protection during updates or for development and testing.

## Pricing

## With Amazon EFS, you pay only for the resources that you use. No minimum fee and no set-up charges are incurred. You pay only for the storage you use for read and write access to data stored in Infrequent Access storage classes and any provisioned throughput. Amazon EFS pricing varies based on the AWS Region where it resides and the storage class. Additional charges apply for Provisioned Throughput.

## For additional information about Amazon EFS pricing, see the Amazon EFS Pricing page on the AWS website.

## File storage: Amazon FSx for Lustre

## Amazon FSx for Lustre streamlines the launching and running of high-performance Lustre file systems. Use FSx for Lustre for workloads where speed matters, such as machine learning, high performance computing (HPC), video processing, and financial modeling.

## Amazon FSx for Lustre

## FSx for Lustre is a managed storage service developed on the open-source, high-performance Lustre file system. 

## The open-source Lustre file system is designed for compute-intensive applications that require a fast storage system capable of meeting throughput requirements. It is also designed to meet input/output operations per second (IOPS) requirements at scale. FSx for Lustre was built to process large datasets quickly and cost-effectively and scale to meet growing demands. An FSx for Lustre file system is capable of delivering hundreds of gibibytes (GiB) per second of throughput and millions of IOPS.

## With FSx for Lustre, you can use the Lustre file system for any workload where speed matters. You do not have the traditional complexity of setting up and managing the Lustre storage system on premises. With FSx for Lustre, you can start your high-performance file system in minutes without the capital investment and operational management expense. 

## Amazon FSx for Lustre is POSIX-compliant, so you can use your current Linux-based applications without having to make any changes. Amazon FSx for Lustre provides a native file system interface and works as any file system does with your Linux operating system. It also provides read-after-write consistency and supports file locking.

## You can integrate FSx for Lustre with Amazon Simple Storage Service (Amazon S3) to process datasets with the FSx for Lustre file system. When linked to an S3 bucket, an FSx for Lustre file system transparently presents S3 objects as files and allows you to write changed data back to Amazon S3.

## With FSx for Lustre, you can scale your compute resources to meet your high-performance compute workload demands. You can scale from hundreds to tens of thousands of CPU cores as your compute processing requires. You can also scale FSx for Lustre to meet your storage capacity and performance requirements.

## Amazon FSx for Lustre features

## High, Scalable Performance

### FSx for Lustre scales using the parallel Lustre file system. The parallel file system adds storage capacity and increases performance linearly as you scale. You can deploy capacity to support hundreds of gibibytes (GiB) per second throughput and millions of IOPS at the same time while maintaining sub-millisecond latencies.

### FSx for Lustre deploys a combination of large memory and storage drive technologies to provide the Lustre file system services for your workloads. The large memory provides the fastest access to optimize performance. 

### FSx for Lustre is deployed using solid state drive (SSD) drives to provide high performance for management operations and serving metadata to your workloads. You can choose between SSD storage or hard disk drive (HDD) storage used to serve data. You choose the baseline throughput performance you need to meet your workload requirements and optimize costs.

### With the built-in Lustre file locking, you can connect tens of thousands of CPU cores to the same storage resources and simultaneously access data as needed by your applications.

### FSx for Lustre provides virtually unlimited resources for your workloads. You can scale to the size you want without the capital expenditures or worrying about expanding your data center footprint. 

### You need only to select the storage capacity and the performance required for your workload.

### To assist you in monitoring your workload performance, FSx for Lustre integrates with Amazon CloudWatch metrics. For more information, see Monitoring Amazon FSx for Lustre in the Amazon FSx for Lustre Users Guide.

## Seamless Access to Data Repositories

## FSx for Lustre appears as a native drive for Amazon Elastic Compute Cloud (Amazon EC2) Linux-based instances and Amazon Elastic Kubernetes Service (Amazon EKS) containers. As a native drive, your applications are able to connect to your FSx for Lustre file system.

## FSx for Lustre natively integrates with your Amazon S3 data repositories. You can read data from your S3 buckets for processing and then output your results to Amazon S3 for low-cost, long-term retention.

## FSx for Lustre supports cloud bursting from your on-premises data repositories. You can import the dataset directly from on premises to FSx for Lustre over AWS Direct Connect or a virtual private network (VPN) connection.

## With native integration, you save time and effort importing your dataset. You also save time exporting your results data from your on-premises storage system for every workload you process.

## Simply and Fully Maganed

## FSx for Lustre is a fully managed AWS storage service. Configuring FSx for Lustre is streamlined using the AWS Management Console. AWS provisions and sets up the servers and storage volumes for your workload. 


## In addition, you can choose to run your FSx for Lustre file system using SSD storage or HDD storage to meet your workload requirements. SSD storage is optimized for latency-sensitive workloads or workloads requiring the highest levels of IOPS and throughput. HDD storage is optimized for throughput-focused workloads that aren’t latency-sensitive. For HDD-based file systems, the optional SSD cache improves performance by placing your most frequently read data on SSD automatically. 

## To optimize your storage costs, long-term data is stored in cost-efficient Amazon S3, in on-premises storage, or in HDD-based FSx for Lustre file systems. 

## When using Amazon S3, data is imported into FSx for Lustre as required by the applications. The data is retained in FSx for Lustre for processing in your workload. The number of Amazon S3 PUT and GET requests to load and save your data are minimized, which helps optimize costs.

## You can launch and delete FSx for Lustre file systems in minutes. As a managed service, FSx for Lustre saves you the time and resource expenses when doing it yourself. Delete any file system you are no longer using when your workload is finished to optimize your costs. 


## AWS configures the Lustre file system and maintains the Lustre software, removing the complexity and maintenance overhead in managing a Lustre file system implementation.

## With the native integration to Amazon S3 and support for cloud bursting from your on-premises data repositories, FSx for Lustre simplifies moving your data into and out of your workload. AWS manages the movement into and out of Amazon S3 for you.

## Native File System Complaint

## FSx for Lustre is POSIX compliant. The FSx for Lustre file system is integrated into the core of the Linux operating system used as part of the service. Because it is POSIX compliant, the FSx for Lustre works as any file system does with your Linux applications. No changes are required to run your applications natively.

## FSx for Lustre maintains read-after-write close consistency for file sharing for your high-performance computing workloads. File locking support is designed into the Lustre file system and is fully supported in FSx for Lustre.

## Cost Optimized

## FSx for Lustre is optimized for performance and low cost. You can choose between the short-term scratch processing option and the longer-term persistent processing options to optimize your costs.

## In addition, you can choose to run your FSx for Lustre file system using SSD storage or HDD storage to meet your workload requirements. SSD storage is optimized for latency-sensitive workloads or workloads requiring the highest levels of IOPS and throughput. HDD storage is optimized for throughput-focused workloads that aren’t latency-sensitive. For HDD-based file systems, the optional SSD cache improves performance by placing your most frequently read data on SSD automatically. 

## To optimize your storage costs, long-term data is stored in cost-efficient Amazon S3, in on-premises storage, or in HDD-based FSx for Lustre file systems. 

## When using Amazon S3, data is imported into FSx for Lustre as required by the applications. The data is retained in FSx for Lustre for processing in your workload. The number of Amazon S3 PUT and GET requests to load and save your data are minimized, which helps optimize costs.

## You can launch and delete FSx for Lustre file systems in minutes. As a managed service, FSx for Lustre saves you the time and resource expenses when doing it yourself. Delete any file system you are no longer using when your workload is finished to optimize your costs. 

## You pay for only the resources you use. You choose how much storage capacity to deploy to meet the dataset size or performance requirements for your workload. You are charged only for the storage capacity and storage performance you select and the time your file system is deployed.

## Secure and Compliant

## FSx for Lustre is integrated into other AWS services for security and compliance. Your data imported into FSx for Lustre is encrypted. No data is openly accessible from an SSD and HDD if one fails or if directly accessed manually. Likewise, your data in your Amazon S3 bucket is encrypted for protection.

## FSx for Lustre is compliant eligible with the following:-

-   Payment card industry (PCI) data security standards (DSS)
-   International Organization for Standardization (ISO)
-   Health Insurance Portability and Accountability Act (HIPAA)

## The systems and software setup used to run the FSx for Lustre service are designed for security. HIPAA compliance is a shared responsibility. Your applications and service security configuration, in addition to the FSx for Lustre service, require certification for compliance.

## You control access to your application using Amazon Virtual Private Cloud (Amazon VPC) security groups. You configure your security groups to allow the access required for only your workload. You configure your VPC to include the resources associated with your workload and allow access from resources in other VPCs, as required.

## You control access using AWS Identity and Access Management (IAM) to set up users, groups, and roles and assign access permissions. IAM access permissions are applied for management and application programming interface (API) access to the FSx for Lustre file system.

## You can monitor and audit API calls using AWS CloudTrail. CloudTrail monitors and logs all API calls to the FSx for Lustre service. You can use these logs for auditing configuration changes and access to the service.

## Amazon FSx for Lustre use cases

## FSx for Lustre provides the performance processing required for compute-intensive workloads across different horizontal and vertical use cases:-

### Horizontal use cases apply across various industries and market segments. These industries have a widespread adoption and ever-increasing demand for more performance to serve increasingly larger number of compute cores. Examples of horizontal use cases include machine learning and high performance computing (HPC) workloads.

### Vertical use cases apply within an industry or market segment. A number of compute-intensive verticals depend on parallel file systems to process workloads. Examples of these workloads include the following:-

-   Life science genomics
-   Financial models
-   Industrial design simulation
-   Media special effects and rendering
-   Seismic and reservoir exploration
-   Any other vertical where HPC and machine language are present


## These are only some of the use cases for FSx for Lustre:-

## Horizontal - Machine Learning

### Machine learning (ML) use cases include applications of Amazon SageMaker, artificial intelligence (AI) and deep learning, autonomous vehicle simulation, and AI/ML batch processing. 

### Machine learning workloads use massive amounts of training data. These workloads often use shared file storage because multiple compute instances need to process the training datasets concurrently. 

### FSx for Lustre is effective for machine learning workloads. For instance, it provides massive parallel shared file storage with high throughput and consistent low latencies to process the machine learning training datasets. You can use FSx for Lustre to speed up your ML training workloads even when data is stored in Amazon S3.

### FSx for Lustre integrates with SageMaker as a direct data source and simplifies your ML workloads.

## Horizontal - High Performance Computing

### Scientists, researchers, and engineers solve complex compute-intensive problems. They typically require a compute profile that uses clusters of computers to drive maximum CPU processing for specialized workloads. 

### High performance computing (HPC) workloads span across machine learning, oil and gas discovery, pharmaceuticals, financial services, and genomics. HPC workloads need to process massive amounts of data. Multiple compute instances with high levels of throughput must be able to access this data. 

### Amazon FSx for Lustre is ideal for HPC workloads because it provides a file system that’s optimized for the performance and costs of performance-intensive workloads. The file system has access across thousands of Amazon EC2 instances and Amazon EKS containers. 

### If you use AWS Batch to manage your HPC compute resource deployment, you can also use it to manage the FSx for Lustre persistent and scratch file systems. You can use AWS Batch to provision the optimal quantity and type of compute resources dynamically. The type and quantity are based on the volume and specific resource requirements of the batch jobs submitted. AWS Batch plans, schedules, and runs your batch computing workloads across AWS compute services and features, such as Amazon EC2 and Spot Instances. 

### You can use AWS ParallelCluster to create a new Amazon FSx for Lustre file system automatically. Alternatively, you can specify an existing Amazon FSx for Lustre file system to use. You can perform any one of these tasks as part of the cluster creation process. 

### The AWS HPC team regularly uses FSx for Lustre as part of their solution stack to help customers in a wide array of disciplines. Part of the solutions is to remove storage as the performance bottleneck and finish workloads much faster.

## Vertical - Genomics and Life Sciences

### Many FSx for Lustre customers are in the life sciences field. Use cases include genomic sequencing, cancer and tumor research, patient therapies, and artificial intelligence.

### Genomics and life sciences workloads use massive amounts of data points. These workloads often use shared file storage accessed by many compute instances that need to process the datasets concurrently. FSx for Lustre reduces the processing time and scales to meet the application high-throughput demands.

### As an example, numerous firms were seeking the fastest possible advances in COVID-19 vaccinations, therapies, and testing. This search resulted in a high demand of FSx for Lustre for genomic sequencing of the virus. 






























