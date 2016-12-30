> ### **Backup and Recovery**

#### 备份数据相关的 AWS 产品

AWS 对数据进行了分级分类，不同类别的数据的备份策略及其对应的 AWS 产品不同。

* **Amazon S3**

  Amazon S3 Standard for general-purpose：面向经常要访问的数据

  Amazon S3 Standard - Infrequent Access：面向需要长期保存，但不经常访问的数据

* **Amazon Glacier**

  面向低成本的，面向长期归档的数据

* **AWS Storage Gateway**

  连接  on-premises 应用到云存储上

* **AWS Transfer Services**

  将客户数据传输到 AWS 云上的多种数据传输服务，比如 AWS Direct Connect, AWS Snowball, AWS Storage Gateway, Amazon S3 Transfer Acceleration

#### 备份和恢复方案设计

AWS 认为备份和恢复策略应该能满足业务的 RTO 和 RPO，需要考虑以下几个方面：

* File-level recovery

* Volume-level recovery

* Application-level recovery \(for example, databases\)

* Image-level recovery

AWS 针对不同类型的应用分别设计了备份和恢复方案，包括面向 cloud native 应用场景，on-premises 应用场景，以及 hybrid 应用场景。

> **cloud native 应用场景**

![](/assets/cloud native-backup.JPG)

数据备份和恢复方案：

* 基于 EBS Snapshot 备份卷和数据

  实现了 File-level 和 Volume-level recovery

* 基于 Database Replica Backups \(Amazon RDS for Backups\)

  实现了 Application-level recovery

* 基于 AMI 备份 EC2 instance

  实现了 Image-level recovery

> **on-premises 应用场景**

数据备份和恢复方案：

* 通过 AWS API 将数据备份到 Amazon S3 和 Glacier （企业内备份软件支持 AWS API 的情况下）

![](/assets/on-premise-backup.JPG)

* 通过 AWS Storage Gateway 将数据备份至 Amazon S3 （企业内备份软件不支持 AWS API 的情况下）

  * Volume gateways

  * Gateway-virtual tape library \(gateway-VTL\)

  ![](/assets/on-premise-connect.JPG)

> **hybrid 应用场景**

数据备份和恢复方案：

* 通过 Direct Connect 连接 on-premises 环境和 AWS 云环境

* AWS-Based Applications 的应用直接将数据备份到 AWS 中

* 将备份管理迁移到云中

* 将长期归档数据放在云中（Amazon Glacier）

  ![](/assets/hybrid-backup.JPG)

> _完整的解决方案请参见_[https://d0.awsstatic.com/whitepapers/Storage/Backup\_and\_Recovery\_Approaches\_Using\_AWS.pdf](https://d0.awsstatic.com/whitepapers/Storage/Backup_and_Recovery_Approaches_Using_AWS.pdf)



