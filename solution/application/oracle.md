> ### **Running Oracle Database on AWS**

在 AWS 上运行 Oracle 数据库的解决方案和最佳实践。



#### 关于数据库 license

方式一：包含在 Amazon RDS License 中，定价包含了Oracle license 的费用，客户无需自己再购买 license；

方式二：Bring Your Own License \(BYOL\)，如果要使用 Oracle Database Enterprise Edition 或 Standard Edition，只能 BYOL。

#### 

#### 如何运行 Oracle 数据库

AWS 提供两种运行数据库的方式供客户选择，使用 Amazon RDS 或者 Amazon EC2，两种方式各有优劣，适合不同场景的需求。



> **方式一：使用 Amazon RDS**

* **优势**：更容易部署、管理和维护，使客户可以更专注在业务层面，而不是日常的数据库管理方面

  Amazon RDS might be a better choice for you if:

  * You want to focus on your business and applications, and have AWS take care of the undifferentiated heavy lifting tasks such as provisioning of the database, management of backup and recovery tasks, management of security patches, minor Oracle version upgrades, and storage management.

  * You need a highly available database solution and want to take advantage of the push-button, synchronous Multi-AZ replication offered by Amazon RDS, without having to manually set up and maintain a standby database.

  * You would like to have synchronous replication to a standby instance for high availability for Oracle Database Standard or Standard One editions.

  * You want to pay for the Oracle license as part of the instance cost on an hourly basis instead of making a large upfront investment.

  * Your database size is less than 6 TB and your maximum IOPS needs are less than 30,000.

  * You do not want to manage backups and, most importantly, point-in-time recoveries of your database.

  * You would rather focus on high-level tasks, such as performance tuning and schema optimization, rather than the daily administration of the database.

  * You want to scale the instance type up and down based on your workload patterns without being concerned about licensing and the complexity involved.

* **劣势**：客户对数据库的控制更少，对数据库底层基础设施的选择灵活性更小



> **方式二：使用 Amazon EC2**

* **优势**：客户对数据库有更多的控制，更加灵活，对数据库底层技术设施有更多的选择

  Amazon EC2 might be a better choice for you if:

  * You need full control over the database, including Sys/System user access, or you need access at the operating system level.

  * Your database size exceeds the 80% of current maximum database size in Amazon RDS, which is 6 TB.

  * You need to use Oracle features or options that are not currently supported by Amazon RDS.

  * Your database IOPS needs are higher than 30,000.

  * You need a specific Oracle Database version that is not supported by Amazon RDS.

* **劣势**：客户需要花更多时间自己完成数据库的日常管理



#### Oracle Database on AWS 架构

更详细的架构设计最佳实践请参考

 [http://d0.awsstatic.com/enterprise-marketing/Oracle/AWSAdvancedArchitecturesforOracleDBonEC2.pdf](http://d0.awsstatic.com/enterprise-marketing/Oracle/AWSAdvancedArchitecturesforOracleDBonEC2.pdf)



> **Enterprise-Class Architecture**

![](/assets/Enterprise-class Oracle.JPG)



> **Large Enterprise-Class Architecture**

![](/assets/large-enterprise-class Oracle.JPG)



> **High-Performance Architecture**

![](/assets/high-performance Oracle.JPG)



> **Oracle RAC Architecture**

![](/assets/Oracle RAC.JPG)

#### Oracle Database on AWS 与 AWS 相关产品

* **安全和网络配置：**

  使用 Amazon VPC 将 Oracle 数据库放在一个私有子网中，并使用安全组和网络 ACL 实现安全策略

* **Amazon EC2 实例类型：**

  如果使用 Amazon RDS，可选的实例类型：

  * db.t2.micro to db.t2.large

  * db.m3.medium to db.m3.2xlarge

  * db.m4.large to db.m4.10xlarge

  * db.r3.large to db.r3.8xlarge

 如果使用 Amazon EC2，可以有更多的实例类型选择，建议选择配置较好的类型，并且要和自己的 Oracle Database 版本对系统配置需求相匹配

 Amazon EC2 实例的选择建议，参见 [http://d0.awsstatic.com/enterprise-marketing/Oracle/AWSAdvancedArchitecturesforOracleDBonEC2.pdf](http://d0.awsstatic.com/enterprise-marketing/Oracle/AWSAdvancedArchitecturesforOracleDBonEC2.pdf)

* **Oracle AMI 选择：**

  可以选择 Oracle 在 AWS 上的官方 AMIs，也可以创建一个只包含操作系统的 Amazon EC2 instance，然后和传统的在硬件设备上部署 Oracle 数据库那样，再将数据库部署到 EC2 上。  
  操作系统的选择建议请参见 [http://d0.awsstatic.com/whitepapers/choosing-os-for-oracle-workloads-on-ec2.pdf](http://d0.awsstatic.com/whitepapers/choosing-os-for-oracle-workloads-on-ec2.pdf)

* **存储选择：**

  由于数据库是读写密集型应用，需要使用高性能磁盘，因此建议选择 Amazon EBS-optimized 实例（系统盘基于 SSD 硬盘）。  
  另外，对于数据盘也有 IOPS 要求，针对不同规模和场景的数据库如何选择存储的建议，参见 [http://d0.awsstatic.com/whitepapers/determining-iops-needs-for-oracle-database-on-aws.pdf](http://d0.awsstatic.com/whitepapers/determining-iops-needs-for-oracle-database-on-aws.pdf)


>_完整的解决方案请参见 https://d0.awsstatic.com/whitepapers/best-practices-for-running-oracle-database-on-aws.pdf_
