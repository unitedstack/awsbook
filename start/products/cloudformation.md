> ### **Amazon CloudFormation**


AWS CloudFormation 向开发人员和系统管理员提供了一种简便地创建和管理一批相关的 AWS 资源的方法，并通过有序且可预测的方式对其进行资源配置和更新。

可以使用 AWS CloudFormation 的示例模板或自己创建模板来介绍 AWS 资源以及应用程序运行时所需的任何相关依赖项或运行时参数。客户无需弄清预配置 AWS 服务的顺序或执行这些依赖关系工作的细微之处。CloudFormation 将进行妥善处理。

部署 AWS 资源后，可以采用可控且可预测的方式修改和更新这些资源，事实上，将版本控制应用到 AWS 基础设施的方法与应用客户的软件的方法相同。还可以使用 AWS CloudFormation Designer 的拖放界面以图表形式显示模板并进行编辑。

可以通过使用 AWS 管理控制台、AWS 命令行接口或 API 对模板及其关联资源集（称为“堆栈”）进行部署和更新。无需为 CloudFormation 支付额外的费用，只需支付支持应用程序 的AWS 资源费用。


#### Amazon CloudFormation 特性


* ##### 广泛支持 AWS 资源

 AWS CloudFormation 支持广泛的 AWS 资源，能够针对应用程序的需求，构建高度可用、可靠且可扩展的 AWS 基础设施。 

* ##### 易于使用

 CloudFormation 使组织和部署 AWS 资源集变得更为轻松，并让客户能够描述任何依赖关系或运行时传入的特殊参数。
 
 可以从许多 CloudFormation 示例模板中选用一个，既可以原样照搬，也可将其作为基础模板予以改造。


* ##### 陈述性和灵活性

 要创建所需的基础设施，只需在 AWS 管理控制台中单击几下、一个命令（使用 AWS 命令行接口）或单个请求（调用 API），在模板中枚举所需的 AWS 资源、配置值和互连关系，然后 AWS CloudFormation 会负责其余所有工作。
 
 不需要记住如何通过服务 API 创建对应的 AWS 资源和建立互连等的细节；AWS CloudFormation 会办妥处理。
 
 如果按照 AWS CloudFormation 自带的多个示例模板之一开始工作，就不需要重新编写模板。


* ##### 基础设施即代码

 一个模板可以重复用于创建同一堆栈的相同副本（或者作为创建新堆栈的基础）。通过模板，可以获知和控制特定于区域的基础设备变化情况，如 Amazon EC2 AMI，以及 Amazon EBS 和 Amazon RDS 快照名称等的变化。
 
 模板是一个简单的 JSON 或 YAML 格式文本文件，可以置于客户的正常源代码控制机制中，存储在 Amazon S3 等私有或公有位置，并能通过电子邮件进行交换。
 
 借助 AWS CloudFormation，客户可以深入了解，以准确地查看哪些 AWS 资源可以形成堆栈。对于作为堆栈一部分而创建的 AWS 资源，客户可以完全控制并改进AWS 资源。


* ##### 通过参数实现自定义

 构建堆栈时，可以使用参数在运行时自定义模板的各个方面。例如，创建堆栈时，可以将 RDS 数据库大小、EC2 实例类型、数据库和 Web 服务器端口号传输到 AWS CloudFormation。也可使用通过参数建立模板创建多个堆栈，以可控制的方式对它们加以区分。
 
 例如，如果客户接收的美国客户流量要比欧洲的多，那么其 Amazon EC2 实例类型、Amazon CloudWatch 警报阈值和 Amazon RDS 只读副本设置可能会在 AWS 地区之间有所不同。可利用模板参数对各个区域中的设置和阈值分别进行小幅调整，但仍需确保各个区域的应用程序的设置是一致的。


* ##### 使用拖放界面显示和编辑

 AWS CloudFormation Designer 可以直观的图表形式显示模板：图标代表 AWS 资源，箭头表示它们之间的关系。可以使用拖放界面构建和编辑模板，然后使用集成的 JSON 文本编辑器编辑模板的详细信息。
 
 CloudFormation Designer 让客户能够将更多的时间花在设计 AWS 基础设施而不是手动编写模板代码上。


* ##### 便于集成
 
 可以将 AWS CloudFormation 与所选的开发和管理工具集成。

 AWS CloudFormation 通过 Amazon Simple Notification Service (SNS) 公布进度事件。借助 SNS，可通过电子邮件跟踪堆栈的创建和删除进度，以及以编程方式和其他流程集成。

