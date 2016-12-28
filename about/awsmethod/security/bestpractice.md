> ### **AWS 最佳实践**

#### 共同责任模型 Shared Responsibility Model

* AWS Secure Global Infrastructure

  IAM

  Regions, AZs, Endpoints

* AWS Services的共同责任模型

  模型概览  
  [https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)  
  ![](/assets/共同责任安全模型.JPG)

  实际上，不同的服务对于 AWS 和客户之间的“分工界面”是不一样的，也就意味着针对不同类型的服务，视 AWS 提供的服务层次和范围，共同责任模型会有所不同。

  * for Infrastructure services

  * for container services

  * for abstracted services

#### 工具

* Trusted Advisor Tool

  参见 Trusted Advisor 产品介绍章节。

#### 一些安全的最佳实践

* AWS账号

  * IAM users

  * IAM Groups

  * IAM Roles

  * AWS Credentials

* EC2在OS层面的访问控制

* 数据安全

  * 访问控制

  * 密钥存储和管理

  * 数据保护

  for S3

  for EBS

  for RDS

  for Glacier

  for DynamoDB

  for EMR

  数据传输安全

  应用和管理者对AWS服务的访问控制

  for 管理AWS服务时的数据传输

  for S3

  for RDS

  for DynamoDB

  for EMR



