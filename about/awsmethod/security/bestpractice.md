> ### **AWS 最佳实践**

#### 共同责任模型 Shared Responsibility Model

* **AWS Secure Global Infrastructure**

  IAM

  Regions, AZs, Endpoints

* **AWS Services的共同责任模型**

  模型概览  
  [https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)  
  ![](/assets/共同责任安全模型.JPG)

  实际上，不同的服务对于 AWS 和客户之间的“分工界面”是不一样的，也就意味着针对不同类型的服务，视 AWS 提供的服务层次和范围，共同责任模型会有所不同。

  * for Infrastructure services

  * for container services

  * for abstracted services

#### 工具

* **Trusted Advisor Tool**

  参见 Trusted Advisor 产品介绍章节。

#### 一些安全的最佳实践

* **AWS账号**

  * IAM users

  * IAM Groups

  * IAM Roles

  * AWS Credentials

* **EC2在OS层面的访问控制**

* **数据安全**

  * 访问控制

  * 密钥存储和管理

  * 数据保护

    * for S3

    * for EBS

    * for RDS

    * for Glacier

    * for DynamoDB

    * for EMR

  * 数据传输安全

    * 应用和管理者对AWS服务的访问控制

    * for 管理AWS服务时的数据传输

    * for S3

    * for RDS

    * for DynamoDB

    * for EMR

* **操作系统和应用安全**

  * AMI

  * bootstrapping

  * 管理 patches

  * 控制公共 AMI 的安全

  * 防恶意软件

  * 减轻危害和滥用

  * 使用额外的应用安全实践

* **基础架构安全**

  * Amazon VPC

  * Security Zoning 和 network segmentation

  * 增强网络安全

  * 用户仓库、DNS、NTP

  * 构建威胁保护层

  * 测试安全

  * 管理指标和改进

  * 减轻和预防DoS & DDoS

* **管理安全的监控、告警、审计、事件响应**

  * 使用变更管理日志

  * 管理关键事务的日志

  * 保护日志信息

  * 记录软件或组件的故障日志



