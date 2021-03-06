This repo will house coursework from the AWS training class from A Cloud Guru for the Solutions Architect Associate Certification as well as course notes.

# Section 2: AWS - 10,000 Feet Overview

This section will cover a top-level overview on the AWS services tested in the Solutions Architect exam.

* AWS officially launched in 2006
* By the numbers, AWS services have grown from 82 in 2011 to over 1300+ in 2017

### Terminology
* What is a Region? A Region is a physical location in the world which consists of two or more AZ's
* What is an AZ? An AZ (Availability Zone) is simply a data center
* What is an Edge Location? Edge Locations are endpoints for AWS which are used for caching content. Typically this consists of CloudFront, Amazon's CDN (Content Delivery Network)

### Compute Service
* EC2 (Elastic Compute Cloud) - Virtual machines inside the AWS platform
* EC2 container service - Run and manage Docker containers at scale
* Elastic Beanstalk - For developers who do not understand AWS who just want to upload their code
* Lambda - A code uploaded to the cloud where you can control when it executes (no need to worry about physical or virtual machine)
* Lightsail - Amazon's VPN (virtual private network) service essentially a watered-down version of EC2
* Batch - Used for batch computing in the cloud

### Storage Service
* S3 (Simple Storage Service) - An object based- storage where we can upload files into buckets in the cloud
* EFS (Elastic File System) - A network-attached service
* Glacier - Data archival service
* Snowball - Way to bring in large amounts of data into the AWS data center
* Storage Gateway - Virtual Machines which will replicate information back to S3

### Database Services
* RDS (Relational Database Service) - Service which works with MySQL, PostgreSQL, Oracle
* DynamoDB - For non-relational databases
* ElastiCache - A way of caching commonly queried items from a database
* Redshift - Built for data warehousing

### Migration Services
* AWS Migration Hub - Tracking service which allows application tracking during migration
* Application Discovery Service - Automated set of tools which not only detects what applications we have but also tracks the dependencies for our application
* Database Migration Service - A way to visualize migrations in action
* Server Migration Service - Helps migrate physical and virtual servers to the cloud
* Snowball - Also a migration tool as well as a storage service

### Networking & Content Delivery
* VPC (Virtual Private Cloud) - Essentially a virtual data center where we can configure things such as firewalls, AZ's, etc.
* CloudFront - Stores information closer to the users and uses a CDN to distribute content on a global scale
* Route 53 - Amazon's DNS service which is highly scaleable
* API Gateway - Is a way of creating our own APIs for our services to talk to
* Direct Connect - A way of running a dedicated line from a data center into Amazon which will directly connect into a VPC

### Developer Tools
* CodeStar - Project management service
* CodeCommit - Source control service or place to store code
* CodeBuild - Once service is ready, this service will compile, run tests, and produce software packages which will enable deployment
* CodeDeploy - Service which automates deployments to EC2 instances, on premise instances, and lambda functions for example
* CodePipeline - Continuous delivery pipeline which will automate the steps required to release software
* X-Ray - Debug service which will help find root causes and performance bottlenecks
* Cloud9 - IDE environment which will allow development on the cloud

### Management Tools
* CloudWatch - Monitoring service
* CloudFormation - Way of scripting infrastructure
* CloudTrail - Used to log changes to the AWS environment (turned on by default and stores logs for a week)
* Config - Monitors the entire AWS environment
* OpsWorks - Similar to Elastic Beanstalk but more robust and is good tool to automate environments
* Service Catalog - A way of managing catalogs of IT services which are approved to use on AWS
* Systems Manager - A resource manager, typically used for EC2
* Trusted Advisor - Will give advice across multiple disciplines
* Managed Services - A manage service for things such as EC2 instances and auto scaling

### Media Services
* Elastic Transcoder - Resizes videos to be compatible on multiple platforms
* MediaConvert - File-based video transcoding service with broadcast grade features
* MediaLive - Broadcast grade video processing service
* MediaPackage - Prepares and protects videos for delivery over the internet
* MediaStore - Storage service optimized for media
* MediaTailor - Allows the ability to do ads on broadcast grade media

### Machine Learning
* SageMaker - Makes it easy to use deep learning
* Comprehend - Sentiment analysis around data
* DeepLens - Artificially aware camera
* Lex - A way of communicating with customers
* Machine Learning - Service to build machine learning projects
* Polly - Takes text and turns it into speech
* Rekognition - Recognizes objects of interest in images and videos
* Amazon Translate - Translation service
* Amazon Transcribe - Transcribe service

### Analytics
* Athena - Allows SQL queries or files in S3 bucket
* EMR (Elastic Map Reduce) - Used for processing large amounts of data
* CloudSearch - Search service for AWS
* ElasticSearch Service - Search service for AWS
* Kinesis - A way of ingesting large amounts of data into AWS
* Kinesis Video Streams - Allows ingesting of large amounts of data from video streams
* QuickSight - Amazon's business intelligence tool
* Data Pipeline - A way of moving data between different AWS services
* Glue - Used for ETL (Extract Transform and Load)

### Security & Identity & Compliance
* IAM (Identity Access Management) - Amazon's IAM service
* Cognito - Device authentication service
* GuardDuty - Monitors for malicious activity on the AWS account
* Inspector - An agent installed on services such as EC2 to check vulnerabilities
* Macie - Scan S3 buckets for PII (Personal Identity Info)
* Certificate Manager - Way of managing SSL certificates
* CloudHSM - Service which offers dedicated bits of hardware used to store keys
* Directory Service - Way of integrating Microsoft active directory services with AWS services
* WAF (Web Application Firewall) - A layer 7 firewall which stops cross-site scripting or SQL injections
* Shield - Service which helps mitigate DDoS attacks
* Artifact - Portal service which allows downloads of compliance reports

### Mobile Services
* Mobile Hub - Management console for mobile apps
* Pinpoint - Uses targeted push notifications to drive mobile engagement
* AWS AppSync - Updates data in web and mobile applications in real-time
* Device Farm - A way of testing apps on real-life devices
* Mobile Analytics - Analytics service for mobile

### AR/VR
* Sumerian - Used for AR, VR and 3D application design, allows you to use a common set of tools to create environments

### Application Integration
* Step Functions - A way of managing different Lambda functions
* Amazon MQ - A way of queuing messages
* SNS (Simple Notification Service) - Notification service if an account goes over some limit
* SQS (Simple Queue Service) - Queue service which is used for decoupling infrastructure
* SWF (Simple Workflow Service) - Workflow service which creates a workflow map for some processes

### Customer Engagement
* Connect - Essentially is a call center in the cloud
* Simple Email Service - Very scaleable service which helps send emails to customers

### Business Productivity
* Alexa For Business - Can use for a variety of business services and tasks
* Chime - Video conferencing similar to Google hangout
* WorkDocs - A drop box for AWS
* WorkMail - Similar to Office 365

### Desktop & App Streaming
* Workspaces - A VDI (virtual desktop infrastructure) solution (running an operating system on AWS cloud)
* AppStream 2.0 - A way to actually stream applications to your desktop

### Internet of Things
* iOT - A way of having thousands or millions of devices sending back data i.e. sensor data such as temperature or humidity to a controller
* iOT Device Management - Used for managing a ton of devices through the AWS service
* Amazon FreeRTOS - Operating system service for microcontrollers
* Greengrass - Software that lets your run local compute, messaging, data caching, sync, and ML inference capabilities for connected devices in a secure way

### Game Development
* GameLift - Service to help develop games in the AWS cloud

## Section 2 Quiz

**1. What is an AWS region?**
* A region is a geographic area that consists of different AZ's. Each region has at least two AZ's.

**2. What does an AWS region consist of?**
* An independent collection of AWS computing resources in a defined geography.

**3. Which statement best describes AZ's?**
* Distinct locations from within an AWS region that are engineered to be isolated form failures.

**4. An AWS VPC is a component of which AWS service?**
* Networking Service

**5. What is a VPC?**
* Virtual Private Cloud

**6. Which AWS service is specifically designed to run a developer's code on an infrastructure that is automatically provisioned to host that code?**
* Elastic Beanstalk

**7. Which AWS service allows you to run code without having to worry about provisioning any underlying resources (such as virtual machines, databases, etc.)**
* Lambda

**8. Amazon's highly scaleable DNS service is known as ________.**
* Route 53

**9. Which AWS compute service is specifically designed to assist you in processing large data sets?**
* Elastic Map Reduce

**10. What is the difference between Elastic Beanstalk & CloudFormation?**
* Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, auto-scaling to application health monitoring based on the code you upload to it, where as CloudFormation is an automated provisioning engine designed to deploy entire cloud environments via a JSON script.

**11. Which AWS service uses a CDN to distribute content around the world?**
* CloudFront

**12. Which of the following AWS solutions offers durable, available storage for flat files?**
* S3

**13. Which of the following AWS services would be the best choice for long term data archival?**
* Glacier

**14. Which AWS service offers the following database engines: SQL, MySQL, MariaDB, PostgreSQL, Aurora, and Oracle?**
* RDS

**15. Which of the following AWS services is used primarily for data warehousing?**
* Redshift

**16. Which AWS service is used for collating large amounts of data streamed from multiple sources?**
* Kinesis

**17. You need to add users to your AWS account and set password rotation policies for these new users. Which AWS service would best fit your requirements?**
* IAM

**18. You need to supply auditors with logs detailing the individual users that provision specific resources on your AWS platform. Which service would best meet this need?**
* CloudTrail

**19. You need a configuration management service that enables your system administrators to configure and operate your web applications using Chef. Which AWS service would best suit your needs?**
* Opsworks

**20. Your digital media agency needs to convert their media files in to different formats to suit different devices. Which AWS service should you consider using to meet these needs?**
* Elastic Transcoder

---

# Section 3: Identity Access Management (IAM)

This section will cover an in-depth overview on the IAM service.

### IAM Overview
* Centralized control of your AWS account
* Shared Access to your AWS account
* Identity Federation (including Active Directory, Facebook, LinkedIn, etc.)
* Multifactor Authentication
* Provide temporary access for users/devices and services where necessary
* Allows you to set up your own password rotation policy
* Integrates with many different AWS services
* Supports PCI DSS Compliance

### Critical Terms
* Users - End Users
* Groups - A collection of users under one set of permissions
* Roles - You create roles and can then assign them to AWS resources
* Policies - A document that defines one (or more permissions)

### IAM - Lab
* IAM does not have a region as it is global
Steps to set up IAM on AWS are as follows:
 1. Delete root access keys
 2. Activate MFA on root account
 3. Create individual IAM users
 4. Use groups to assign permissions
 5. Apply an IAM password policy
* IAM roles are a secure way to grant permissions to entities that you trust.

### Create a Billing Alarm - Lab
* We can create a billing alarm by navigating to CloudWatch and configuring alarms for billing

### What Have We Learned?
* IAM consists of the following:
 1. Users
 2. Groups
 3. Roles
 4. Policy Documents
* IAM is universal, it does not apply to regions at this time
* The "root account" is simply the account created on AWS account setup. This account has complete Admin access
* New users have no permissions when first created
* New users are assigned Access Key ID and Secret Access Keys when first created
* Access Key ID & Secret Access Keys are not the same as a password and you cannot use them to login to the console. You can use these keys to access AWS via the APIs and CLI however
* You only get to view the Access Key ID & Secret Access Keys once. If lost will need to be regenerated.
* Always setup MFA (Multifactor Authentication) on the root account
* It is possible to create and customize the password rotation policies

## Section 3 Quiz

**1. Which statement best describes IAM**
* IAM Allows you to manage users, groups, roles, and their corresponding level of access to the AWS platform

**2. Which of the following is NOT a feature of IAM?**
* Allows you to set biometric authentication, so that no passwords are required

**3. Power User Access allows ___**
* Access to all AWS services except for management of groups and users within IAM

**4. What level of access does the "root" account have?**
* Administrator Access

**5. You are a solutions architect working for a large engineering company who are moving their existing legacy hardware to AWS. You have configured their first AWS account and you have set up IAM. Your company will be primarily based out of West Germany, however they will have a small subsidiary operating out of South Korea and you will need an AWS environment configured there as well. Which of the following statements is true;**
* You will need to configure Users and Policy Documents only once, as these are applied globally

**6. You have a client who is considering moving to AWS services and do not yet have an account. What is the first thing the company should do to set up an AWS Account?**
* Set up an account using their company email address

**7. You are a security administrator working for a hotel chain. You have a new member of staff who has started as a systems administrator and they will need full access to the AWS console. You have created the user account and generated the access key id and the secret access key. You have moved this user into the group where the other administrators are and you have provided the new user with their secret access key and their access key id. However when they go to log in to the AWS console, they cannot sign in. What could be the cause of this?**
* You cannot log in to the AWS console using the Access Key ID and Secret Access Key, instead you must generate a password for the user and supply the user with this password, as well as the unique link to sign in to the AWS console

**8. What is an additional way to secure IAM for both the root login and new users alike?**
* Implement MFA for all accounts

**9. By default when you create a new user in the IAM console, what level of access do they have?**
* No access to all AWS services

**10. In what language are policy documents written in?**
* JSON

---

# Section 4: AWS Object Storage and CDN - S3, Glacier and CloudFront

This section will cover an in-depth overview on the S3 (Simple Storage Service) service.

### What is S3?
* S3 provides developers and IT teams with secure, durable, highly-scalable object storage. Amazon S3 is easy to use, with a simple web services interface to store and retrieve any amount of data from anywhere on the web
* S3 is a safe place to store your files
* S3 is an object-based storage
* The data is spread across multiple devices and facilities

### S3 - The Basics
* S3 is Object-based - i.e. allows you to upload files
* Files can be from 0 Bytes to 5 TB
* There is unlimited storage
* Files are stored in Buckets
* S3 is a universal namespace - names must be unique globally
* URLs look like https://s3-eu-west-1.amazonaws.com/<name>
* When you upload a file to S3 you will receive a HTTP 200 code if the upload was successful

### Data Consistency Model for S3
* Read after Write consistency for PUTS of new Objects
* Eventual Consistency for overwrite PUTS and DELETES (can take some time to propagate)

### S3 is a Simple Key-value Store
Objects consist of the following:
 * Key (this is the name of the object)
 * Value (this is the data and is made up of a sequence of bytes)
 * Version ID (important for versioning)
 * Metadata (Data about data you are storing)
 * Sub resources:
    * Access Control Lists
    * Torrent

### S3 - The Basics (Continued)
* Built for 99.99% availability for the S3 platform.
* Amazon guarantee 99.9% availability
* Amazon guarantee 99.99999999999% durability for S3 information (11 x 9s)
* Tiered storage available
* Lifecycle Management
* Versioning
* Encryption
* Secure your data using Access Control Lists and Bucket Policies

### S3 - Storage Tiers/Classes
* S3 Standard: 99.99% availability, 99.9999999999% durability, stored redundantly across multiple devices in multiple facilities, and is designed to sustain the loss of 2 facilities concurrently
* S3 - IA: (Infrequently Accessed): For data that is accessed less frequently, but requires rapid access when needed. Lower fee than S3 but you are charged a retrieval fee
* S3 One Zone - IA: Want a lower-cost option for infrequently accessed data but do not require the multiple AZ data resilience
* Glacier: Very cheap but used for archival only. Expedited, Standard or Bulk. A standard retrieval time takes 3-5 hours

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/s3-storage-tiers.jpg">
  <h3>Figure 4-1. S3 Storage classes and info</h3>
</div>

### S3 - Charges
In S3, we are charged for:
* Storage
* Requests
* Storage Management Pricing
* Data Transfer Pricing
* Transfer Acceleration

### What is S3 Transfer Acceleration?
AWS S3 Transfer Acceleration enables fast, easy, and secure transfers of files over long distances between your end users and an S3 bucket. Transfer Acceleration takes advantage of AWS CloudFront's globally distributed edge locations. As the data arrives at an edge location, data is routed to AWS S3 over an optimized network path.

### Create and S3 Bucket - Exam Tips
* Buckets are a universal name space
* Upload an object to S3 receives a HTTP 200 code on success
* S3, S3-IA, S3 Reduced Redundancy Storage
* Encryption
  * Client Side Encryption
  * Server Side Encryption
    * Server side encryption with Amazon S3 Managed Keys (SSE-S3)
    * Server side encryption with KMS (SSE-KMS)
    * Server side encryption with Customer Provided Keys (SSE-C)
* Control access to buckets using either a bucket ACL or using Bucket Policies
* **By default buckets are private and all objects stored inside them are private**

### S3 - Versioning Exam Tips
* Stores all versions of an object (including all writes and even if you delete an object)
* Great backup tool
* Once enabled, versioning cannot be disabled, only suspended
* Integrates with Lifecycle rules
* Versioning's MFA Delete capability, which uses multi-factor authentication, can be used to provide an additional layer of security

### S3 - Cross Region Replication Exam Tips
* Versioning must be enabled on both the source and destination buckets
* Regions must be unique
* Files in an existing bucket are not replicated automatically. All subsequent updated files will be replicated automatically
* You cannot replicate to multiple buckets or use daisy chaining
* Delete markers are replicated
* Deleting individual versions or delete markers will not be replicated
* Understand what Cross Region Replication is at a high level

### S3 - Lifecycle Management Lab
* Can be used in conjunction with versioning
* Can be applied to current versions and previous versions
* Following actions can now be done:
  * Transition to the Standard - Infrequent Access Storage Class (30 days after creation date)
  * Archive to the Glacier Storage Class (30 days after IA)
  * Permanently Delete

### What is a CDN?
A CDN (content delivery network) is a system of distributed servers (network) that delivers webpages and other web content to a user based on the geographic locations of the user, the origin of the webpage and a content delivery server.

### CloudFront - Key Terms
* Edge Location - The location where content will be cached. This is separate to an AWS region/AZ
* Origin - The origin of all the files that the CDN will distribute. This can be either an S3 Bucket, an EC2 Instance, and Elastic Load Balancer or Route 53
* Distribution - The name given the CDN which consists of a collection of Edge Locations

### What is CloudFront?
Amazon CloudFront can be used to deliver your entire website, including dynamic, static, streaming, and interactive content using a global network of edge locations. Requests for your content are automatically routed to the nearest edge location, so content is delivered with the best possible performance.

Amazon CloudFront is optimized to work with other services such as S3, EC2, Elastic Load Balancing, and Route 53. CloudFront also works seamlessly with any non-AWS origin server, which stores the original, definitive versions of your files.

### CloudFront - Key Terms (Continued)
* Web Distribution - Typically used for websites
* RTMP - Used for media streaming

### CloudFont - Exam Tips
* Understand the key terms: Edge Location, Origin, Distribution, Web Distribution, and RTMP
* Edge locations are not just READ only, you can write to them too
* Objects are cached for the life of the TTL (time to live)
* You can clear cached objects but you will be charged

### Securing your buckets
* By default, all newly created buckets are **private**
* You can setup access control to your buckets using:
  * Bucket Policies
  * Access Control Lists
* S3 buckets can be configured to create access logs which log all requests made to the S3 bucket. This can be done to another bucket

### Encryption
There are four types of Encryption for S3:
* In transit:
  * SSL/TLS
* At rest:
  * Server Side Encryption
    * S3 Managed Keys - SSE-S3
    * AWS Key Managed Service, Managed Keys - SSE-KMS
    * Server Side Encryption with Customer Provided Keys - SSE-C
  * Client Side Encryption

### Storage Gateway
AWS Storage Gateway is a service that connects an on-premises software appliance with cloud-based storage to provide seamless and secure integration between an organization's on-premises IT environment and AWS's storage infrastructure. The service enables you to securely store data to the AWS cloud for scalable and cost-effective storage.

AWS Storage Gateway's software appliance is available for download as a VM (virtual machine) image that you install on a host in your data center. Storage Gateway supports either VMware ESXi or Microsoft Hyper-V. Once you've installed your gateway and associated it with your AWS account through the activation process, you can use the AWS Management Console to create the storage gateway option that is right for you.

### Four Types of Storage Gateways
* File Gateways (NFS)
* Volumes Gateway (iSCSI)
  * Stored Volumes
  * Cached Volumes
* Tape Gateway (VTL)

### File Gateway
Files are stored as objects in your S3 buckets, accessed through a Network File System (NFS) mount point. Ownership, permissions, and timestamps are durably stored in S3 in the user-metadata of the object associated with the file. Once objects are transferred to S3, they can be managed as native S3 objects, and bucket policies such as versioning, lifecycle management, and cross-region replication apply directly to objects stored in your bucket.

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/s3-file-gateway.jpg">
  <h3>Figure 4-2. Sample S3 file gateway architecture</h3>
</div>

### Volume Gateway
The volume interface presents your applications with disk volumes using the iSCSI block protocol

Data written to these volumes can be asynchronously backed up as point-in-time snapshots of your volumes, and stored in the cloud as Amazon EBS snapshots.

Snapshots are incremental backups that capture only changed blocks. All snapshot storage is also compressed to minimize your storage charges.

### Volume Gateway - Stored Volumes
Stored volumes let your primary data locally, while asynchronously backing up that data to AWS. Stored volumes provide your on-premises applications with low-latency access to their entire datasets, while providing durable, off-site backups. You can create storage volumes and mount them as iSCSI devices from your on-premises application servers. Data written to your stored volumes is stored on your on-premises storage hardware. This data is asynchronously backed up to S3 in the form of EBS (Amazon Elastic Block Store) snapshots. 1GB - 16 TB in size for Stored Volumes.

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/volume-gateway-stored-volumes.jpg">
  <h3>Figure 4-3. Sample S3 volume gateway stored volumes architecture</h3>
</div>

### Volume Gateway - Cached Volumes
Cached volumes let you use S3 as your primary data storage while retaining frequently access data locally in your storage gateway. Cached volumes minimize the need to scale your on-premises storage infrastructure, while still providing your applications with low-latency access to their frequently accessed data. You can create storage volumes up to 32 TB in size and attached to them as iSCSI devices from your on-premises application servers. Your gateway stores data that you write to these volumes in S3 and retains recently read data in your on-premises storage gateway's cache and upload buffer storage. 1 GB - 32 TB in size for Cache Volumes

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/volume-gateway-cached-volumes.jpg">
  <h3>Figure 4-4. Sample S3 volume gateway cached volume architecture</h3>
</div>

### Volume Gateway - Tape Gateway
Tape Gateway offers a durable, cost-effective solution to archive your data in the AWS Cloud. The VTL interface it provides lets your leverage your existing tape-based backup application infrastructure to store data on virtual tape cartridges that you create on your tape gateway. Each tape gateway is preconfigured with a media changer and tape drives, which are available to your existing client backup applications as ISCSI devices. You add tape cartridges as your need to archive your data. Supported by NetBackup, Backup Exec, Veeam etc.

<div align="center">
  <img src="Section 04 -- AWS Object Storage and CDN - S3, Glacier and CloudFront/volume-gateway-tape-gateway.jpg">
  <h3>Figure 4-5. Sample S3 volume gateway tape gateway architecture</h3>
</div>

### Storage Gateway - Exam Tips
* File Gateway - For flat files, stored directly on S3
* Volume Gateway:
  * Stored Volumes - Entire dataset is stored on site and is asynchronously backed up to S3
  * Cached Volumes - Entire dataset is stored on S3 and the most frequently accessed data is cached on site
* Gateway Virtual Tape Library (VTL)
  * Used for backup and uses popular backup applications like NetBackup, Backup Exec, Veeam etc.

### Import/Export Disk
AWS Import/Export Disk accelerates moving large amounts of data into and out of the AWS cloud using portable storage devices for transport. AWS Import/Export Disk transfers your data directly onto and off of storage devices using Amazon's high-speed internal network and bypassing the Internet.

### Types of Snowballs
* Snowball
* Snowball Edge
* Snowmobile

### Snowball
* Snowball is a petabyte-scale data transport solution that uses secure appliances to transfer large amounts of data into and out of AWS. Using Snowball addresses common challenges with large-scale data transfers including high network costs, long transfer times, and security concerns. Transferring data with Snowball is simple, fast, secure, and can be as little as one-fifth the cost of high-speed Internet.

80 TB snowball in all regions. Snowball uses multiple layers of security designed to protect your data including tamper-resistant enclosures, 256-bit encryption, and an industry-standard Trusted Platform Module (TPM) designed to ensure both security and full chain-of-custody of your data. Once the data transfer job has been processed and verified, AWS performs a software erasure of the Snowball appliance.

### Snowball Edge
AWS Snowball Edge is a 100 TB data transfer device with on-board storage and compute capabilities. You can use Snowball Edge to move large amounts of data into and out of AWS, as a temporary storage tier for large local datasets, or to support local workloads in remote or offline locations.

Snowball Edge connects to your existing applications and infrastructure using standard storage interfaces, streamlining the data transfer process and minimizing setup and integration. Snowball Edge can cluster together to form a local storage tier and process your data on-premises, helping ensure your applications continue to run even when they are not able to access the cloud.

### Snowmobile
AWS Snowmobile is an Exabyte-scale data transfer service used to move extremely large amounts of data to AWS. You can transfer up to 100 PB per Snowmobile, a 45-foot long ruggedized shipping container, pulled by a semi-trailer truck. Snowmobile makes it easy to move massive volumes of data to the cloud, including video libraries, image repositories, or even a complete data center migration. Transferring data with Snowmobile is secure, fast, and cost effective.

### Snowball - Exam Tips
* Understand what Snowball is
* Understand what Import/Export is
* Snowball can:
  * Import to S3
  * Export to S3

### What is S3 Transfer Acceleration?
S3 Transfer Acceleration utilizes the CloudFront Edge Network to accelerate your uploads to S3. Instead of uploading directly to your S3 bucket, you can use a distinct URL to upload directly to an edge location which will then transfer that file to S3. You will get a distinct URL to upload to.

### Summary
* Know the core fundamentals of S3:
  * Key (name)
  * Value (data)
  * Version ID
  * Metadata
  * Access control lists
* Object based storage only (for files)
* **Not suitable to install an operating system on**
* Remember that S3 is Object based i.e. allows you to upload files
* Files can be from 0 bytes to 5 TB
* There is unlimited storage
* Files are stored in buckets
* S3 is a universal namespace, that is, names must be unique globally
* Sample URL: https://s3-eu-west-1.amazonaws.com/<name>
* Read after Write consistency for PUTS of new Objects
* Eventual Consistency for overwrite PUTS and DELETES (can take some time to propagate)

#### Summary - S3 Storage Tiers/Classes
* Know the different storage tiers/classes:
  * S3 Standard
  * S3-IA
  * S3 One Zone-IA
  * Glacier

#### Summary - S3 Versioning
* Stores all versions of an object (including all writes and even if you delete an object)
* Great backup tool
* Once enabled, cannot be disabled, only suspended
* Integrates with Lifecycle rules
* Versioning's MFA Delete capability, which uses multi-factor authentication, can be used to provide an additional layer of security
* Cross Region Replication, requires versioning enabled on the source bucket

#### Summary - S3 Lifecycle Management
* Can be used in conjunction with versioning
* Can be applied to current versions and previous versions
* Following actions can now be done:
  * Transition to the Standard - Infrequent Access Storage Class (128 Kb and 30 days after the creation date)
  * Archive to the Glacier Storage Class (30 days after IA, if relevant)
  * Permanently Delete

#### Summary - CloudFront
* Edge Location - This is the location where content will be cached. This is separate to an AWS AZ
* Origin - This is the origin of all the files that the CDN will distribute. This can be either an S3 Bucket, an EC2 Instance, an Elastic Load Balancer or Route 53
* Distribution - This is the name given the CDN which consists of a collection of Edge Locations. There are different types:
  * Web Distribution - Typically used for websites
  * RTMP - Used for media streaming
* Edge locations are not just READ only, you can write to them too
* Objects are cached for the life of the TTL (Time to Live)
* You can clear cached objects but you will be charged

#### Summary - Securing your buckets
* By default, all newly created buckets are PRIVATE
* You can setup access control to your buckets using:
  * Bucket Policies
  * Access Control Lists
* S3 buckets can be configured to create access logs which log all requests made to the S3 bucket. This can be done to another bucket

#### Summary - Encryption
* In Transit:
  * SSL/TLS
* At Rest:
  * Server Side Encryption
    * S3 Managed Keys - SSE-S3
    * AWS Key Management Service, Managed Keys - SSE-KMS
    * Server Side Encryption with Customer Provided Keys - SSE-C
  * Client Side Encryption

#### Summary - Storage Gateway
* File Gateway - For flat files, stored directly on S3
* Volume Gateway:
  * Stored Volumes - Entire dataset is stored on site and is asynchronously backed up to S3
  * Cached Volumes - Entire dataset is stored on S3 and the most frequently accessed data is cached on site
* Gateway Virtual Tape Library (VTL)
  * Used for backup and uses popular backup applications like NetBackup, Backup Exec, Veeam etc.

#### Summary - Snowball
Types of snowball:
* Snowball
* Snowball Edge
* Snowmobile

#### Summary - S3 Transfer Acceleration
* You can speed up transfers to S3 using S3 transfer acceleration. This costs extra and has the greatest impact on people who are in a faraway location

#### S3 Static Websites
* You can use S3 to host static websites
* Serverless
* Very cheap, scales automatically
* STATIC only, cannot host dynamic sites

#### Summary - Last Few Tips
* Write to S3 - HTTP 200 code for a successful write
* You can load files to S3 much faster by enabling multipart upload
* Read the S3 FAQ before taking the exam. It comes up A LOT!

## Section 4 Quiz

**1. S3 has what consistency model for PUTS of new objects**
* Read After Write Consistency

**2. What is AWS Storage Gateway?**
It's an on-premise virtual appliance that can be used to cache S3 locally at a customer’s site

**3. One of your users is trying to upload a 7.5GB file to S3 however they keep getting the following error message - "Your proposed upload exceeds the maximum allowed object size.” What is a possible solution for this?**
* Design your application to use the multi-part upload API for all objects

**4. What does RRS stand for when talking about S3?**
* Reduced Redundancy Storage

**5. You have been asked by your company to create an S3 bucket with the name "acloudguru1234" in the EU West region. What would be the URL for this bucket?**
* https://s3-eu-west-1.amazonaws.com/acloudguru1234

**6. What is Amazon Glacier?**
* An AWS service designed for long term data archival

**7. What does S3 stand for?**
* Simple Storage Service

**8. You are a solutions architect who works with a large digital media company. The company has decided that they want to operate within the Japanese region and they need a bucket called "testbucket" set up immediately to test their web application on. You log in to the AWS console and try to create this bucket in the Japanese region however you are told that the bucket name is already taken. What should you do to resolve this?**
* Bucket names are global, not regional. This is a popular bucket name and is already taken. You should choose another bucket name

**9. What is the availability on RRS?**
* 99.99%

**10. What is the durability on RRS?**
* 99.99%

**11. What is the durability on S3?**
* 99.999999999%

**12. What is the availability on S3?**
* 99.99%

**13. What is the minimum file size that I can store on S3?**
* 0 bytes

**14. The difference between S3 and EBS is that EBS is object based where as S3 is block based.
* False

**15. S3 has eventual consistency for which HTTP Methods?**
* Overwrite PUTS and Deletes

**16. You work for a busy digital marketing company who currently store their data on premise. They are looking to migrate to AWS S3 and to store their data in buckets. Each bucket will be named after their individual customers, followed by a random series of letters and numbers. Once written to S3 the data is rarely changed, as it has already been sent to the end customer for them to use as they see fit. However on some occasions, customers may need certain files updated quickly, and this may be for work that has been done months or even years ago. You would need to be able to access this data immediately to make changes in that case, but you must also keep your storage costs extremely low. The data is not easily reproducible if lost. Which S3 storage class should you choose to minimize costs and to maximize retrieval times?**
* S3-IA

**17. You need to use an Object based storage solution to store your critical, non-replaceable data in a cost effective way. This data will be frequently updated and will need some form of version control enabled on it. Which S3 storage solution should you use?**
* S3

**18. You work for a health insurance company who collects large amounts of documents regarding patients’ health records. This data will be used usually only once when assessing a customer and will then need to be securely stored for a period of 7 years. In some rare cases you may need to retrieve this data within 24 hours of a claim being lodged. Which storage solution would best suit this scenario? You need to keep your costs as low as possible.**
* Glacier

**19. You run a meme creation website that frequently generates meme images. The original images are stored in S3 and the meta data about the memes are stored in DynamoDB. You need to store the memes themselves in a low cost storage solution. If an object is lost, you have created a Lambda function that will automatically recreate this meme using the original file in S3 and the metadata in DynamoDB. Which storage solution should you consider to store this non-critical, easily reproducible data on in the most cost effective solution as possible?**
* S3-RRS

**20. You run a popular photo sharing website that is based off S3. You generate revenue from your website via paid for adverts, however you have discovered that other websites are linking directly to the images on your site, and not to the HTML pages that serve the content. This means that people are not seeing your adverts and every time a request is made to S3 to serve an image it is costing your business money. How could you resolve this issue?**
* Remove the ability for images to be served publicly to the site and then use signed URLs with expiry dates

---

# Section 5: EC2 - The Backbone of AWS

This section will cover an in-depth overview on the AWS Elastic Compute Cloud (EC2) service.

### What is EC2?
Amazon EC2 (Elastic Cloud Compute) is a web service that provides resizable compute capacity in the cloud. Amazon EC2 reduces the time required to obtain and boot new server instances to minutes, allowing you to quickly scale capacity, both up and down, as your computing requirements change.

EC2 changes the economics of computing by allowing you to pay only for capacity that you actually use. EC2 provides developers the tools to build failure resilient applications and isolate themselves from common failure scenarios.

### EC2 Options
* On Demand - Allows you to pay a fixed rate by the hour (or by the second) with no commitment
* Reserved - Provides you with a capacity reservation and offers a significant discount on the hourly charge for an instance. 1 year or 3 year terms
* Spot - Enables you to bid whatever price you want for instance capacity, providing for even greater savings if your applications have flexible start and end times
* Dedicated Hosts - Physical EC2 server dedicated for you use. Dedicated Hosts can help you reduce costs by allowing you to use your existing server-bound software licenses

### On Demand
* Perfect for users that want the low cost and flexibility of EC2 without any up-front payment or long-term commitment
* Applications with short term, spiky, or unpredictable workloads that cannot be interrupted
* Applications being developed or tested on EC2 for the first time

### Reserved
* Applications with steady state or predictable usage
* Applications that require reserved capacity
* Users can make up-front payments to reduce their total computing costs even further
  * Standard RIs (up to 75% off on-demand)
  * Convertible RIs (up to 54% off on-demand) feature the capability to change the attributes of the RI as long as the exchange results in the creation of Reserved Instances of equal or greater value
  * Schedule RIs are available to launch within the time window you reserve. This option allows you to match your capacity reservation to a predictable recurring schedule that only requires a fraction of a day, week, or month

### Spot
* Applications that have flexible start and end times
* Applications that are only feasible at very low compute prices
* Users with an urgent need for large amounts of additional computing capacity

### Dedicated Hosts
* Useful for regulatory requirements that may not support multi-tenant virtualization
* Great for licensing which does not support multi-tenancy or cloud deployments
* Can be purchased on-demand (hourly)
* Can be purchased as a Reservation for up to 70% off the on-demand price

### EC2 Instance Types

<div align="center">
  <img src="Section 05 -- EC2 - The Backbone of AWS/specialities-use-cases.jpg">
  <h3>Figure 5-1. EC2 instance types, specialties and use cases</h3>
</div>

### What is EBS?
Amazon EBS (Elastic Block Storage) allows you to create storage volumes and attach them to EC2 instances. Once attached, you can create a file system on top of these volumes, run a database, or use them in any other way you would use a block device. EBS volumes are placed in a specific AZ where they are automatically replicated to protect you from the failure of a single component.

### EBS Volume Types
* General Purpose SSD (GP2)
  * General purpose, balances both price and performance
  * Ratio of IOPS per GB with up to 10,000 IOPS and the ability to burst up to 300 IOPS for extended periods of time for volumes at 3334 GB and above
* Provisioned IOPS SSD (101)
  * Designed for I/O intensive applications such as large relational or NoSQL databases
  * Use if you need more than 10,000 IOPS
  * Can provision up to 20,000 IOPS per volume
* Throughput Optimized HDD (ST1)
  * Big data
  * Data warehouses
  * Log processing
  * Cannot be a boot volume
* Cold HDD (SC1)
  * Lowest cost storage for infrequently accessed workloads
  * File server
  * Cannot be a boot volume
* Magnetic (Standard)
* Lowest cost per GB of all EBS volume types that is bootable. Magnetic volumes are ideal for workloads where data is accessed infrequently, and applications where the lowest storage cost is important

### EC2 Exam Tips
* Know On-Demand, Reserved, Spot, and Dedicated Host EC2 services
* If a Spot instance is terminated by EC2, you will not be charged for a partial hour of usage. However, if you terminate the instance yourself, you will be charged for the complete hour in which the instance ran
* Know FIGHT DR MC PX acronym (EC2 instance types, specialties and use cases)
* SSD:
  * General Purpose SSD - Balance price and performance for a wide variety of workloads
  * Provisioned IOPS SSD - Highest performance SSD volume for mission-critical low-latency or high-throughput workloads

* Magnetic:
  * Throughput Optimized HDD - Low cost HDD volume designed for frequently accessed, throughput-intensive workloads
  * Cold HDD - Lowest cost HDD volume designed for less frequently accessed workloads
  * Magnetic - Previous generation. Can be boot volume

### EC2 Lab Summary
* Termination Protection is turned off by default, you must turn it on
* On an EBS-backed instance, the default action is for the root EBS volume to be deleted when the instance is terminated
* EBS root volumes of your DEFAULT AMI's cannot be encrypted. You can also use a third party tool (such as bit locker) to encrypt the root volume, or this can be done when creating AMI's in the AWS console or using the API

### Security Group Basics
* All inbound traffic is blocked by default
* All outbound traffic is allowed
* Changes to security groups take effect immediately
* You can have any number of EC2 instances within a security group
* You can have multiple security groups attached to EC2 instances
* Security groups are STATEFUL (network access control lists are STATELESS):
  * If you create an inbound rule allowing traffic in, that traffic is automatically allowed back out again
* You cannot block specific IP addresses using security groups, instead use Network Access Control Lists
* You can specify allow rules but not deny rules

### Volumes and Snapshots
* Volumes exist on EBS:
  * Virtual Hard Disk
* Snapshots exist on S3
* Snapshots are point in time copies of volumes
* Snapshots are incremental - this means that only the blocks that have changed since your last snapshot are moved to S3

### Snapshots of Root Device Volumes
* To create a snapshot for EBS volumes that serve as root devices, you should stop the instance before taking the snapshot
* However, you can take while the instance is running
* You can create AMI's from EBS-backed instances and snapshots
* You can change EBS volume sizes on the fly, including changing the size and storage type
* Volumes will ALWAYS be in the same AZ as the EC2 instance
* To move an EC2 volume from one AZ/Region to another, take a snap or an image of it, then copy it to the new AZ/Region

### Volume vs Snapshots - Security
* Snapshots of encrypted volumes are encrypted automatically
* Volumes restored from encrypted snapshots are encrypted automatically
* You can share snapshots, but only if they are unencrypted
  * These snapshots can be shared with other AWS accounts or made public

### RAID, Volumes and Snapshots
* RAID - Redundant Array of Independent Disks
  * RAID 0 - Striped, No Redundancy, Good Performance
  * RAID 1 - Mirrored, Redundancy
  * RAID 5 - Good for reads, bad for writes, AWS does not recommend ever putting RAID 5's on EBS
  * RAID 10 - Striped and Mirrored, Good Redundancy, Good Performance

### Snapshots of a RAID array
* Problem - Take a snapshot, the snapshot excludes data held in the cache by applications and the OS. This tends not to matter on a single volume, however using multiple volumes in a RAID array, this can be a problem due to interdependencies of the array
* Solution - Take an application consistent snapshot
  * Stop the application from writing to disk
  * Flush all caches to the disk
  * Ways to accomplish these tasks above:
    * Freeze the file system
    * Unmount the RAID array
    * Shutting down the associated EC2 instance

### EBS vs Instance Store
* All AMIs are categorized as either backed by EBS or backed by instance store
* For EBS volumes - The root device for an instance launched from the AMI is an EBS volume created from an EBS snapshot
* For instance store volumes - The root device for an instance launched from the AMI is an instance store volume created from a template stored in S3

### EBS vs Instance Store - Exam Tips
* Instance store volumes are sometimes called Ephemeral Storage
* Instance store volumes cannot be stopped. If the underlying host fails, you lose your data
* EBS backed instance can be stopped. You will not lose the data on this instance if it is stopped
* You can reboot both, you will not lose your data
* By default, both ROOT volumes will be deleted on termination, however with EBS volumes, you can tell AWS to keep the root device volume

### Types of Load Balancers
Three types of load balancers:
* Application load balancer - Are best suited for load balancing of HTTP and HTTPS traffic. They operate at Layer 7 and are application-aware. They are intelligent, and you can create advanced request routing, sending specified requests to specific web servers
* Network load balancer - Are best suited for load balancing of TCP traffic where extreme performance is required. Operating at the connection level (Layer 4), network load balancers are capable of handling millions of requests per second, while maintaining ultra-low latencies. Use for extreme performance
* Classic load balancer - Are the legacy ELB (Elastic Load Balancers). You can load balance HTTP/HTTPS applications and use Layer 7-specific features, such as X-Forwarded and sticky sessions. You can also use strict Layer 4 load balancing for applications that rely purely on the TCP protocol

### Load Balancer Errors
* Classic Load Balancers - If your application stops responding the ELB responds with a 504 error. This means that the application is having issues. This could be either at the Web Server layer or at the Database Layer. Identify where the application is failing and scale it up or out where possible

### ELB Exam Tips
* 3 types of load balancers:
  * Application load balancers
  * Network load balancers
  * Classic load balancers
* 504 error means that the gateway has timed out. This means that the application not responding within the idle timeout period.
  * Trouble shoot the application. Is it the Web Server or Database Server?
* If you need the IPv4 address of your end user, look for the X-Forwarded-For-Header

### Elastic Load Balancers Lab
* Instances monitored by ELB are reported as “In Service” or “Out of Service”
* Health Checks - Check the instance health by talking to it
* ELBs have their own DNS name. You are never given an IP address
* Read the ELB FAQ for Classic Load Balancers

### CloudWatch EC2 Lab
* Standard Monitoring - 5 minute
* Detailed Monitoring - 1 minute
* What can I do with CloudWatch?
  * Dashboards - Create awesome dashboards to see what is happening with your AWS environment
  * Alarms - Allows you to set Alarms that notify you when particular thresholds are hit
  * Events - CloudWatch events helps you respond to state changes in your AWS resources
  * Logs - CloudWatch logs helps you aggregate, monitor, and store logs

### The AWS Command Line and EC2
* When we configure AWS via command line we are actually storing credentials locally on the EC2 instance
* Using user credentials is not safe and storing them on EC2 instances is not recommended

### Using IAM roles with EC2
* Roles help secure credentials in AWS EC2
* Remember that all roles are global so there is no need to create a new role in another Region

### S3 CLI and Regions
* You can now actually attach a role to an EC2 instance via CLI or AWS console

### Using Bootstrap Scripts
* Bash scripts are always passed in the Advanced Details tab
* We use #!/bin/bash to start the bash script
* Bash scripts allows us to automate our web servers

### EC2 Instance Metadata
Instance metadata is data about your instance that you can use to configure or manage the running instance. Instance metadata is divided into categories.

Although you can only access instance metadata and user data from within the instance itself, the data is not protected by cryptographic methods. Anyone who can access the instance can view its metadata. Therefore, you should take suitable precautions to protect sensitive data (such as long-lived encryption keys). You should not store sensitive data, such as passwords, as user data.

You can also use instance metadata to access user data that you specified when launching your instance. For example, you can specify parameters for configuring your instance, or attach a simple script. You can also use this data to build more generic AMIs that can be modified by configuration files supplied at launch time. For example, if you run web servers for various small businesses, they can all use the same AMI and retrieve their content from the Amazon S3 bucket you specify in the user data at launch. To add a new customer at any time, simply create a bucket for the customer, add their content, and launch your AMI. If you launch more than one instance at the same time, the user data is available to all instances in that reservation.

EC2 instances can also include dynamic data, such as an instance identity document that is generated when the instance is launched.

For more information on EC2 instance metadata see the AWS EC2 guide on [Instance Metadata and User Data](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-metadata.html).

### Autoscaling Lab
An important take away is that you can have instances spread across multiple AZs and even if you lose two of those AZ out of three you still won't have an outage. Route 53 can also help further protect from regional failure by detecting failure and redirecting traffic to other parts of the world.

### EC2 Placement Groups
There are two types of placement groups:
* Clustered Placement Group - A grouping of instances within a single AZ. Placement groups are recommended for applications that need low network latency, high network throughput, or both. Only certain instances can be launched into a clustered placement group
* Spread Placement Group - A group of instances that are each placed on distinct underlying hardware. Spread placement groups are recommended for applications that have a small number of critical instances that should be kept separate from each other

Things to review before the exam:
* A clustered placement group can't span multiple AZ
* A spread placement group can span multiple AZ
* The name you specify for a placement group must be unique within your AWS account
* Only certain types of instances can be launched in a placement group (Compute Optimized, GPU, Memory Optimized, Storage Optimized)
* AWS recommend homogenous instances within placement groups
* You can't merge placement groups
* You can't move an existing instance into a placement group. You can create an AMI from your existing instance, and then launch a new instance from the AMU into a placement group

### What is EFS?
Amazon EFS (Elastic File System) is a file storage service for Amazon EC2 instances. Amazon EFS is easy to use and provides a simple interface that allows you to create and configure file systems quickly and easily. With EFS, storage capacity is elastic, growing and shrinking automatically as you add and remove files, so your applications have the storage they need, when they need it.

### EFS Features
* Supports the Network File System version 4 (NFSv4) protocol
* You only pay for the storage you use (no pre-provisioning required)
* Can scale up to the petabytes
* Can support thousands of concurrent NFS connections
* Data is stored across multiple AZ's within a region
* Read After Write Consistency

Use case for EFS:
* Using EFS as a file server or a central repository for your files within your EC2 instances
* Can set restrictions which will be reflected across all EC2 instances
* EFS allows multiple EC2 instances to connect to it whereas EBS can only mount to a single EC2 instance

### What is Lambda?
AWS Lambda is a compute service where you can upload your code and create a Lambda function. AWS Lambda takes care of provisioning and managing the servers that you use to run the code. You don't have to worry about operating systems, patching, scaling, etc. You can use Lambda in the following ways:

* As an event-driven compute service where the AWS Lambda runs your code in response to events. These events could be changes to data in an Amazon S3 bucket or an Amazon DynamoDB table
* As a compute service to run your code in response to HTTP requests using Amazon API Gateway or API calls made using AWS SDKs

Lambda is an encapsulation of the following:
* Data Centers
* Hardware
* Assembly Code/Protocols
* High Level Languages
* Operating Systems
* Application Layer/AWS APIs
* AWS Lambda

### How is Lambda Priced?
* Number of requests:
  * First 1 million requests are free. $0.20 per 1 million requests thereafter
* Duration:
  * Calculated from the time your code begins executing until it returns or otherwise terminates, rounded up to the nearest 100 ms. The price depends on the amount of memory you allocate to your function. You are charged $0.00001667 for every GB-second used

### Why is Lambda Cool?
* No servers!
* Continuous scaling!
* Super cheap!

### Lambda - Exam Tips
* Lambda scales out (not up) automatically
* Lambda functions are independent, 1 event = 1 function
* Lambda is serverless
* Know what services are serverless!
* Lambda function can trigger other lambda functions, 1 event can = x functions if functions trigger other functions

* Architectures can get extremely complicated, AWS X-ray allows you to debug what is happening
* Lambda can do things globally, you can use it to back up S3 buckets to other S3 buckets etc.
* Know triggers

### Build a Serverless Page
Below is a schematic of how the lambda serverless website will work with Route 53, API Gateway, Lambda, and S3. The steps are as follows:

1. Get IP address
2. Route 53 returns IP address
3. Get web page from S3
4. Return static/dynamic content
5. Get request to API Gateway
6. Forward request to Lambda
7. Return data to user

<div align="center">
  <img src="Section 05 -- EC2 - The Backbone of AWS/lambda-serverless-web.jpg">
  <h3>Figure 5-2. Lambda serverless web schematic</h3>
</div>

### Using Polly
Below is a schematic of how Polly will be set up in AWS. Polly converts text into an MP3 file.

<div align="center">
  <img src="Section 05 -- EC2 - The Backbone of AWS/polly-setup.jpg">
  <h3>Figure 5-3. Overview of Polly application</h3>
</div>

### EC2 Summary
Below are the major subsections in Section 5 worth going over before the exam.

#### Exam Tips - EC2
* Know the differences between:
  * On Demand
  * Spot
  * Reserved
  * Dedicated Hosts
* Remember with spot instances:
  * If you terminate the instance, you pay for the hour
  * If AWS terminates the spot instance, you get the hour it was terminated in for free

* Know the EC2 instance types as shown in Figure 5-1

#### Exam Tips - EBS
* EBS Consists of:
  * SSD, General Purpose - GP2 - (up to 10,000 IPOS)
  * SSD, Provisioned IOPS - IO1 - (more than 10,000 IOPS)
  * HDD, Throughput Optimized - ST1 - Frequently accessed workloads
  * HDD, Cold - SC1 - Less frequently accessed data
  * HDD, Magnetic - Standard - Cheap, infrequently accessed storage

* You cannot mount a single EBS volume to multiple EC2 instances; instead use EFS

#### Exam Tips - EC2 Lab
* Termination Protection is turned off by default, you must turn it on
* On an EBS-backed instance, the default action is for the root EBS volume to be deleted when the instance is terminated
* EBS-backed root volumes can now be encrypted using AWS API or console or you can use a third party tool to encrypt the root volume
* Additional volumes can also be encrypted

#### Exam Tips - Volumes vs Snapshots
* Volumes exist on EBS:
  * Virtual hard disk
* Snapshots exist on S3
* You can take a snapshot of a volume, this will store that volume on S3
* Snapshots are point in time copies of volumes
* Snapshots are incremental. This means that only the blocks that have changed since your last snapshot are moved to S3
* It may take some time to create the first snapshot

#### Exam Tips - Volumes vs Snapshots - Security
* Snapshots of encrypted volumes are encrypted automatically
* Volumes restored from encrypted snapshots are encrypted automatically
* You can share snapshots, but only if they are unencrypted
  * These snapshots can be shared with other AWS accounts or made public

#### Exam Tips - Snapshots of Root Device Volumes
* To create a snapshot for Amazon EBS volumes that serve as root devices, you should stop the instance before taking the snapshot

#### Exam Tips - EBS vs Instance Store
* Instance store volumes are sometimes called Ephemeral Storage
* Instance store volumes cannot be stopped. If the underlying host fails, you lose your data
* EBS backed instance can be stopped. You will not lose the data on this instance if it is stopped
* You can reboot both, you will not lose your data
* By default, both ROOT volumes will be deleted on termination, however with EBS volumes, you can tell AWS to keep the root device volume

### How to take Snapshots of a RAID array
* Problem - Take a snapshot, the snapshot excludes data held in the cache by applications and the OS. This tends not to matter on a single volume, however using multiple volumes in a RAID array, this can be a problem due to interdependencies of the array
* Solution - Take an application consistent snapshot
  * Stop the application from writing to disk
  * Flush all caches to the disk
  * Ways to accomplish these tasks above:
    * Freeze the file system
    * Unmount the RAID array
    * Shutting down the associated EC2 instance

#### Exam Tips - Amazon Machine Images
AMIs are regional. You can only launch an AMI from the region in which it is stored. However you can copy AMIs to other regions using the console, command line, or the Amazon EC2 API

#### Exam Tips - CloudWatch Lab
* Standard Monitoring - 5 minute
* Detailed Monitoring - 1 minute

* CloudWatch is performance monitoring
* CloudTrail is for auditing

#### What can I do with CloudWatch?
  * Dashboards - Create awesome dashboards to see what is happening with your AWS environment
  * Alarms - Allows you to set Alarms that notify you when particular thresholds are hit
  * Events - CloudWatch events helps you respond to state changes in your AWS resources
  * Logs - CloudWatch logs helps you aggregate, monitor, and store logs

#### Exam Tips - Roles Lab
* Roles are more secure than storing your access key and secret access key on individual EC@ instances
* Roles are easier to manage
* Roles can be assigned to an EC2 instance AFTER it has been provisioned using both the command line and the AWS console
* Roles are universal - you can use them in any region

#### Exam Tips - Instance Metadata
* Used to get information about an instance (such as public IP)

#### Exam Tips - EFS Lab
* Supports the Network File System version 4 (NFSv4) protocol
* You only pay for the storage you use (no pre-provisioning required)
* Can scale up to the petabytes
* Can support thousands of concurrent NFS connections
* Data is stored across multiple AZ's within a region
* Read After Write Consistency

#### What is Lambda?
AWS Lambda is a compute service where you can upload your code and create a Lambda function. AWS Lambda takes care of provisioning and managing the servers that you use to run the code. You don't have to worry about operating systems, patching, scaling, etc. You can use Lambda in the following ways:

* As an event-driven compute service where the AWS Lambda runs your code in response to events. These events could be changes to data in an Amazon S3 bucket or an Amazon DynamoDB table
* As a compute service to run your code in response to HTTP requests using Amazon API Gateway or API calls made using AWS SDKs

#### What is a Placement Group?
There are two types of placement groups:
* Clustered Placement Group - A grouping of instances within a single AZ. Placement groups are recommended for applications that need low network latency, high network throughput, or both. Only certain instances can be launched into a clustered placement group
* Spread Placement Group - A group of instances that are each placed on distinct underlying hardware. Spread placement groups are recommended for applications that have a small number of critical instances that should be kept separate from each other

## Section 5 Quiz

**1. EBS Snapshots are backed up to S3 in what manner?**
* Incrementally

**2. Do Amazon EBS volumes persist independently from the life of an Amazon EC2 instance, for example, if I terminated an EC2 instance, would that EBS volume remain?**
* Only if instructed to when created

**3. Can I delete a snapshot of an EBS Volume that is used as the root device of a registered AMI?**
* No, you must deregister the AMI before being able to delete the root device

**4. A placement group can be deployed across multiple Availability Zones.**
* False

**5. While creating the snapshots using the command line tools, which command should I be using?**
* ec2-create-snapshot

**6. Can you attach an EBS volume to more than one EC2 instance at the same time?**
* No

**7. A placement group is ideal for**
* EC2 instances that require high network throughput and low latency across a single AZ

**8. Using the console, I can add a role to an EC2 instance, after that instance has been created and powered up.**
* True

**9. I can change the permissions to a role, even if that role is already assigned to an existing EC2 instance, and these changes will take effect immediately.**
* True

---
