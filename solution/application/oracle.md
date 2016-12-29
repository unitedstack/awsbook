> ### **Running Oracle Database on AWS**

在 AWS 上运行 Oracle 数据库的解决方案和最佳实践。

#### 关于数据库 license

方式一：包含在 Amazon RDS License 中，定价包含了Oracle license 的费用，客户无需自己再购买 license；

方式二：Bring Your Own License (BYOL)，如果要使用 Oracle Database Enterprise Edition 或 Standard Edition，只能 BYOL。


#### 如何运行 Oracle 数据库

AWS 提供两种运行数据库的方式供客户选择，使用 Amazon RDS 或者 Amazon EC2，两种方式各有优劣，适合不同场景的需求。

>**方式一：使用 Amazon RDS**

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

>**方式二：使用 Amazon EC2**

* **优势**：客户对数据库有更多的控制，更加灵活，对数据库底层技术设施有更多的选择

 Amazon EC2 might be a better choice for you if:

 * You need full control over the database, including Sys/System user access, or you need access at the operating system level.

 * Your database size exceeds the 80% of current maximum database size in Amazon RDS, which is 6 TB.

 * You need to use Oracle features or options that are not currently supported by Amazon RDS.
 
 * Your database IOPS needs are higher than 30,000.

 * You need a specific Oracle Database version that is not supported by Amazon RDS.

* **劣势**：客户需要花更多时间自己完成数据库的日常管理

####  Oracle Database on AWS 架构








