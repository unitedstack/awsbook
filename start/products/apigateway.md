> ### **Amazon API Gateway**


Amazon API Gateway 是一种完全托管的服务，可以帮助开发者轻松创建、发布、维护、监控和保护任意规模的 API。

只需在 AWS 管理控制台中点击几下，便可以创建可充当应用程序“前门”的 API，从后端服务访问数据、业务逻辑或功能，例如基于 Amazon Elastic Compute Cloud (Amazon EC2) 运行的工作负载、基于 AWS Lambda 运行的代码或任意 Web 应用。

Amazon API Gateway 负责管理所有任务，涉及接受和处理成千上万个并发 API 调用，包括流量管理、授权和访问控制、监控以及 API 版本管理。

Amazon API Gateway 没有最低费用或启动成本，只需为收到的 API 调用和传输出去的数据量付费。


#### AWS API Gateway 特性

* ##### 降低成本并提高效率

 借助 Amazon API Gateway，只需为 API 调用以及传输出去的数据量付费。无最低费用，无预先承诺。


* ##### 任意规模都能高效使用

 借助于 Amazon CloudFront 集成，API Gateway 能够利用全球范围的边缘位置网络为最终用户提供尽可能低的 API 请求和响应延迟。此外，Amazon API Gateway 还可帮助客户通过限制规则来管理流量，以便后端操作可以经受住流量峰值的考验。此外，Amazon API Gateway 还可通过缓存 API 调用的输出内容来避免不必要的后端系统调用，从而帮助客户提高 API 的绩效


* ##### 轻松监控 API 活动

 在 API 部署后，Amazon API Gateway 会提供控制面板，以便客户可以使用 Amazon CloudWatch 直观地监控服务的调用，从而查看 API 调用的性能指标和相关信息、数据延迟以及错误率。


* ##### 简化 API 开发

 Amazon API Gateway 使客户可以同时运行同一 API 的多个版本，从而能够快速迭代、测试和发布新版本。 


* ##### 灵活的安全控制机制

 API Gateway 可为客户提供可以授权访问 API 和控制服务操作的工具。可以使用多种 AWS 管理和安全工具（比如 AWS Identity and Access Management (IAM) 和 Amazon Cognito）来对 API 的访问进行授权。Amazon API Gateway 可以使用 AWS 用于自身 API 的技术来代表您验证签名的 API 调用。如果已在使用 OAuth 令牌或其他授权机制，则 Amazon API Gateway 可以使用 AWS Lambda 执行自定义授权命令，以便验证传入请求。


* ##### 为现有服务创建 RESTful 端点

 通过 Amazon API Gateway，可以基于新式资源创建新的 API，然后使用灵活的动态数据转换功能以客户的目标服务希望使用的语言生成请求。API Gateway 还可设置限制规则来避免在不可预测的流量峰值期间耗尽后端基础设施资源，从而帮助客户保护现有服务的安全。


* ##### 无服务器运行 API

 Amazon API Gateway 与 AWS Lambda 紧密集成，可以创建完全无服务器的 API。通过 Amazon API Gateway，可创建基于 REST 的 API，移动和 Web 应用均可使用这些 API 通过 AWS Lambda 中运行的代码来调用公开提供的 AWS 服务。AWS Lambda 在高可用性计算基础设施上运行代码，用于执行所有繁重工作以及计算资源进行管理。