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





























