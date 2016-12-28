## AWS产品之间的关系


几个基石：

EC2：

大部分的计算任务基于 EC2 实例。

Amazon EC2 与 Amazon Simple Storage Service \(Amazon S3\)、Amazon Relational Database Service \(Amazon RDS\)、Amazon SimpleDB 和 Amazon Simple Queue Service \(Amazon SQS\) 配合使用，为多种应用程序提供完整的计算、查询处理和存储解决方案。


VPC：除了提供丰富的网络功能，也是实现云中安全性的重要组件

S3：

是很多服务的基础，数据是企业及其业务的核心和生命力，而 S3 作为重要的数据存储产品，完成了对数据从存储到分析、从备份到灾难恢复等多个关键场景的支持。

Amazon S3 与其他 AWS 服务深度集成，因此客户很容易构建基于 Amazon S3 使用各种 AWS 服务的解决方案。集成的服务包括 Amazon CloudFront、Amazon CloudWatch、Amazon Kinesis、Amazon RDS、Amazon Glacier、Amazon EBS、Amazon DynamoDB、Amazon Redshift、Amazon Route 53、Amazon EMR、Amazon VPC、Amazon KMS 和 AWS Lambda。

CloudWatch：通过监控数据的收集和传递，完成和实现了  监控运维、为 data-driven 的云架构优化提供基础，为使用审计和合规性提供基础，为各种自动化操作提供基础，为在云上实践传统企业 ITIL 流程中的事件管理提供基础。是一个非常重要的管道。