> ### **Amazon EC2**

Amazon Elastic Compute Cloud \(Amazon EC2\) 是一种 Web 服务，可在云中提供大小可调的计算容量。该服务旨在降低开发人员进行网络规模级云计算的难度。

Amazon EC2 的 Web 服务接口非常简单，可以轻松获取和配置容量。使用该服务，可以完全控制自己的计算资源，并可以在成熟的 Amazon 计算环境中运行。

Amazon EC2 将获取并启动新服务器实例所需要的时间缩短至几分钟，这样一来，在计算要求发生变化时，便可以快速扩展计算容量。

Amazon EC2 按实际使用的容量收费，从而改变了成本结算方式。 Amazon EC2 还为开发人员提供了创建故障恢复应用程序以及排除常见故障情况的工具。

#### Amazon EC2 特性

* ##### 弹性 Web 规模级计算

可以在几分钟 \(而不是几小时或几天\) 内增加或减少容量。可以同时管理一个、数百个，甚至数千个服务器实例。这全是通过 Web 服务 API 控制，所以客户的应用程序可根据其自身需要自动扩展。

* ##### 完全控制

客户可以完全控制自己的实例。客户拥有每个实例的管理员或根用户访问权，可以像与其他任何机器一样与这些实例互动。可以在停止运行实例的同时将数据保存在启动分区，然后用 Web 服务 API 重启。使用 Web 服务 API 还可以远程重启实例。还拥有实例控制台输出的访问权。

* ##### 灵活的云托管服务

有多种实例类型、操作系统和软件包供选择。可以为选择的操作系统和应用程序选取理想的内存、CPU、实例存储和启动分区大小配置。例如，可选的操作系统包括许多 Linux 发行版和 Microsoft Windows Server。

EC2 实例类型：https://aws.amazon.com/ec2/instance-types/

Amazon AMI： https://aws.amazon.com/marketplace/b/2649367011?ref_=hmpg_categories_2649367011

* ##### 专为与其他 Amazon Web Services 配合使用而设计

Amazon EC2 与 Amazon Simple Storage Service \(Amazon S3\)、Amazon Relational Database Service \(Amazon RDS\)、Amazon SimpleDB 和 Amazon Simple Queue Service \(Amazon SQS\) 配合使用，为多种应用程序提供完整的计算、查询处理和存储解决方案。

* ##### 可靠

Amazon EC2 提供了一个非常可靠的环境，替代实例可在此环境中快速并以可预见的方式启动。该服务在成熟的 Amazon 网络基本架构和数据中心中运行。Amazon EC2 服务等级协议的承诺是为每个 Amazon EC2 区域提供 99.95% 的可用性。

* ##### 安全

Amazon EC2 与 Amazon VPC 配合工作，为客户的计算资源提供安全及强大的联网功能。

计算实例位于 Virtual Private Cloud \(VPC\) 中，它具有指定的 IP 范围。可以决定哪些实例向互联网公开，哪些实例保持私有状态。

安全组和网络 ACL 能控制进入和离开客户的实例的入站和出站网络访问。

可以通过工业标准的加密 IPsec VPN 连接，将客户现有的 IT 基础设施关联到 VPC 中的资源。

有关更多隔离，可以在专用主机上预配置 EC2 资源或预配置为专用实例。这两种方法都可让客户在专供单个客户使用的硬件上的 VPC 中使用 EC2 实例。

如果没有默认 VPC，则必须创建一个 VPC 并将实例推送到该 VPC 以利用各种高级的联网功能，例如私有子网、出站安全组过滤、网络 ACL、专用实例和 VPN 连接。

