## AWS产品体系

Amazon Web Services 提供了大量基于云的全球性产品，其中包括计算、存储、数据库、分析、联网、移动产品、开发人员工具、管理工具、物联网、安全性和企业级应用程序。这些服务可帮助组织快速发展、降低 IT 成本以及进行扩展。很多大型企业和热门的初创公司都通过这些服务为各种工作负载提供技术支持，其中包括 Web 和移动应用程序、游戏开发、数据处理与仓库、存储、存档及很多其他工作负载。

AWS 并不显式的从 IaaS、PaaS、SaaS 角度来划分产品体系，因为在他们看来，所有的产品是为满足业务需求而服务的，客户关心的是如何解决业务问题，而不是这些产品处于 Infrastructure / Platform / Software 的哪个层次。

通过 AWS 丰富的产品类别和产品，可以看出 AWS 是如何理解各种企业的业务场景，如何理解企业内不同用户的使用需求，并且如何通过产品服务来满足这些场景和需求的。

![](/assets/产品体系.JPG)

完整的产品介绍请参考 AWS 官方链接：

[https://aws.amazon.com/cn/products/?nc2=h\_ql\_ny\_gsc](https://aws.amazon.com/cn/products/?nc2=h_ql_ny_gsc)

> ### **计算**

* Amazon EC2

  云中的虚拟服务器

* Amazon EC2 Container Registry

  存储和检索 Docker 映像

* Amazon EC2 Container Service

  运行和管理 Docker 容器

* Amazon Lightsail

  启动和管理虚拟专有服务器

* Amazon VPC

  隔离的云资源

* AWS Batch

  运行任意规模的批处理作业

* AWS Elastic Beanstalk

  运行和管理 Web 应用

* AWS Lambda

  运行代码以响应事件

* Auto Scaling

  自动化弹性扩展

> ### **存储**

* Amazon S3

  云中的可扩展存储

* Amazon EBS

  针对 EC2 进行块存储

* Amazon Elastic File System

  针对 EC2 进行托管文件存储

* Amazon Glacier

  云中的低成本归档存储

* AWS Storage Gateway

  混合存储集成

* AWS Snowball

  PB 级数据传输

* AWS Snowball Edge

  通过板载计算实现 PB 级数据传输

* AWS Snowmobile

  EB 级数据传输

> ### **数据库**

* Amazon Aurora

  高性能的托管关系数据库

* Amazon RDS

  适用于 MySQL、PostgreSQL、Oracle、SQL Server 和 MariaDB 的托管关系数据库服务

* Amazon DynamoDB

  托管 NoSQL 数据库

* Amazon ElastiCache

  内存中的缓存系统

* Amazon Redshift

  快速简单、经济高效的数据仓库

* AWS Database Migration Service

  以最少停机时间迁移数据库

> ### **迁移**

* AWS Database Migration Service

  以最少停机时间迁移数据库

* AWS Server Migration Service

  将本地服务器迁移到 AWS

* AWS Snowball

  PB 级数据传输

* AWS Snowball Edge

  通过板载计算实现 PB 级数据传输

* AWS Snowmobile

  EB 级数据传输

> ### **网络和内容分发**

* Amazon VPC

  隔离的云资源

* Amazon CloudFront

  全球内容分发网络

* Amazon Route 53

  可扩展域名系统

* AWS Direct Connect

  AWS 专用网络连接

* Elastic Load Balancing

  高扩展负载均衡

> ### **开发人员工具**

* AWS CodeCommit

 在私人 Git 存储库中存储代码

* AWS CodeBuild

 生成和测试代码

* AWS CodeDeploy

 自动化代码部署

* AWS CodePipeline

 使用连续交付发布软件

AWS X-Ray

分析和调试应用程序

AWS 命令行界面

用于管理 AWS 服务的统一工具

> ### **管理工具**

Amazon CloudWatch  
监控资源和应用程序  
Amazon EC2 Systems Manager  
配置和管理 EC2 实例和本地服务器  
AWS CloudFormation  
使用模版来创建和管理资源  
AWS CloudTrail  
追踪用户活动和 API 使用情况  
AWS Config  
追踪资源库存和变更  
AWS OpsWorks  
利用 Chef 自动化操作  
AWS Service Catalog  
创建和使用标准化产品  
AWS Trusted Advisor  
优化性能和安全性  
AWS Personal Health Dashboard  
AWS 服务运行状况的个性化视图

> ### **安全性、身份与合规性**

AWS Identity & Access Management  
管理用户权限和加密密钥  
Amazon Inspector  
分析应用程序安全性  
AWS Certificate Manager  
预置、管理和部署 SSL/TLS 证书  
AWS CloudHSM  
有助于实现监管合规性的基于硬件的密钥存储  
AWS Directory Service  
托管和管理 Active Directory  
AWS Key Management Service  
管理型的密钥创建和控制  
AWS Organizations  
管理多个账户的设置  
AWS Shield  
DDoS 保护  
AWS WAF  
过滤恶意 Web 流量

> ### **分析**

Amazon Athena  
使用 SQL 在 S3 中查询数据  
Amazon EMR  
托管的 Hadoop 框架  
Amazon CloudSearch  
托管的搜索服务  
Amazon Elasticsearch Service  
运行和扩展 Elasticsearch 集群  
Amazon Kinesis  
处理实时流式数据  
Amazon Redshift  
快速简单、经济高效的数据仓库  
Amazon Quicksight  
高速商业分析服务  
AWS Data Pipeline  
适用于周期性数据驱动工作流的编排服务  
AWS Glue  
准备和加载数据

> ### **人工智能**

Amazon Lex  
构建语音和文本聊天机器人  
Amazon Polly  
将文本转换为逼真的语音  
Amazon Rekognition  
搜索和分析图像

> ### **移动服务**

AWS Mobile Hub  
构建、测试和监控应用程序  
Amazon API Gateway  
构建、部署和管理 API  
Amazon Cognito  
用户身份和应用程序数据同步  
Amazon Pinpoint  
为移动应用程序推送通知  
AWS Device Farm  
在云中的真实设备上测试 Android, FireOS 和 iOS 应用程序  
AWS 移动软件开发工具包  
移动软件开发工具包

> ### **应用程序服务**

AWS Step Functions  
协调分布式应用程序  
Amazon API Gateway  
构建、部署和管理 API  
Amazon Elastic Transcoder  
易用型可扩展媒体转码

> ### **消息收发**

Amazon SQS  
消息队列服务  
Amazon SNS  
推送通知服务  
Amazon Pinpoint  
为移动应用程序推送通知  
Amazon SES  
电子邮件发送和接收服务

> ### **企业生产力**

Amazon WorkDocs  
企业存储和共享服务  
Amazon WorkMail  
安全和托管的商业电子邮件和日历编排

> ### **桌面和应用程序流式处理**

Amazon WorkSpaces  
桌面计算服务  
Amazon AppStream 2.0  
将桌面应用程序流式传输至浏览器

> ### **物联网**

AWS IoT 平台  
将设备连接到云  
AWS Greengrass  
本地计算、消息收发和设备同步  
AWS IoT Button  
可编程的云端 Dash Button

> ### **游戏开发**

Amazon Lumberyard  
一种免费的跨平台 3D 游戏引擎，与 AWS 和 Twitch 集成，提供完整源代码

