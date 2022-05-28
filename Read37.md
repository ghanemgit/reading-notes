# Amazon Simple Storage Service(S3)

### What is Amazon S3?
#### Amazon Simple Storage Service (Amazon S3) is a scalable, high-speed, web-based cloud storage service. The service is designed for online backup and archiving of data and applications on Amazon Web Services (AWS). Amazon S3 was designed with a minimal feature set and created to make web-scale computing easier for developers.

### Amazon S3 features
#### S3 provides 99.999999999% durability for objects stored in the service and supports multiple security and compliance certifications. An administrator can also link S3 to other AWS security and monitoring services, including CloudTrail, CloudWatch and Macie. There's also an extensive partner network of vendors that link their services directly to S3.

#### Data can be transferred to S3 over the public internet via access to S3 application programming interfaces (APIs). There's also Amazon S3 Transfer Acceleration for faster movement over long distances, as well as AWS Direct Connect for a private, consistent connection between S3 and an enterprise's own data center. An administrator can also use AWS Snowball, a physical transfer device, to ship large amounts of data from an enterprise data center directly to AWS, which will then upload it to S3.

#### In addition, users can integrate other AWS services with S3. For example, an analyst can query data directly on S3 either with Amazon Athena for ad hoc queries or with Amazon Redshift Spectrum for more complex analyses.

### Amazon S3 use cases
#### Amazon S3 can be used by organizations ranging in size from small businesses to large enterprises. S3's scalability, availability, security and performance capabilities make it suitable for a variety of data storage use cases. Common use cases for S3 include the following:

- data storage;
- data archiving;
- application hosting for deployment, installation and management of web apps;
- software delivery;
- data backup;
- disaster recovery (DR);
- running big data analytics tools on stored data;
- data lakes;
- mobile applications;
- internet of things (IoT) devices;
- media hosting for images, videos and music files; and
- website hosting -- particularly well suited to work with Amazon CloudFront for content delivery.

### How Amazon S3 works
#### Amazon S3 is an object storage service, which differs from other types of cloud computing storage types, such as block and file storage. Each object is stored as a file with its metadata included. The object is also given an ID number. Applications use this ID number to access objects. This is unlike file and block cloud storage, where a developer can access an object via a representational state transfer (REST) API.

#### The S3 object storage cloud service gives a subscriber access to the same systems that Amazon uses to run its own websites. S3 enables customers to upload, store and download practically any file or object that is up to 5 terabytes (TB) in size -- with the largest single upload capped at 5 gigabytes (GB).


### Amazon S3 storage classes
#### Amazon S3 comes in seven storage classes:

- S3 Standard
is suitable for frequently accessed data that needs to be delivered with low latency and high throughput. 
- S3 Standard 
targets applications, dynamic websites, content distribution and big data workloads.
- S3 Intelligent-Tiering 
is most suitable for data with access needs that are either changing or unknown. S3 Intelligent-Tiering has four different access tiers: Frequent Access, Infrequent Access (IA), Archive and Deep Archive. Data is automatically moved to the most inexpensive storage tier according to customer access patterns.
- S3 Standard-IA 
offers a lower storage price for data that is needed less often but that must be quickly accessible. This tier can be used for backups, DR and long-term data storage.
- S3 One Zone-IA 
is designed for data that is used infrequently but requires rapid access on the occasions that it is needed. Use of S3 One Zone-IA is indicated for infrequently accessed data without high resilience or availability needs, data that is able to be recreated and backing up on-premises data.
- S3 Glacier 
is the least expensive storage option in S3, but it is strictly designed for archival storage because it takes longer to access the data. Glacier offers variable retrieval rates that range from minutes to hours.
- S3 Glacier 
Deep Archive has the lowest price option for S3 storage. S3 Glacier Deep Archive is designed to retain data that only needs to be accessed once or twice a year.
- S3 Outposts 
adds S3 object storage features and APIs to an on-premises AWS Outposts environment. S3 Outposts is best used when performance needs call for data to be stored near on-premises applications or to satisfy specific data residency requirements.
#### A user can also implement lifecycle management policies to curate data and move it to the most appropriate tier over time.
