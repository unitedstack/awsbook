> ### **Web Application Hosting **

面向 Web Application Hosting 的应用解决方案由如下 AWS 产品和服务组成：

![](/assets/webapplication.JPG)

* **Route 53**: 提供 DNS 服务

* **Elastic Load Balancer**: 为 Web Server Autoscaling 组做负载转发和均衡

* **Amazon EC2 and Auto Scaling**:

  * Web 层自动伸缩组， 一组 EC2 instances 组成，处理 HTTP 请求

  * App Server Load Balancer, 运行在 EC2 上的软件负载均衡 \(如 HAProxy），对 app server 集群做负载转发

  * App 层自动伸缩组， 一组运行实际应用的 EC2 instances 组成，EC2 实例属于自动伸缩组

* **ElastiCache**: 为应用提供缓存，减轻数据库层的负载

* **CloudFront**: 提供 CDN 服务

* **MySQL RDS DB**: 数据库层，跨 AZ 部署成高可用架构。也可以针对多读应用创建只读副本来分散访问流量

* **Amazon S3**: 用于备份和存放静态对象数据

* **Host Security**: 通过 Amazon EC2 的安全组来提供主机安全

> _完整的解决方案请参见 _[https://d0.awsstatic.com/whitepapers/aws-web-hosting-best-practices.pdf](https://d0.awsstatic.com/whitepapers/aws-web-hosting-best-practices.pdf)



