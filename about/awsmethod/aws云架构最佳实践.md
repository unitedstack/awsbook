## AWS 云架构最佳实践


> ### **云计算与传统 IT 的区别 **

* **IT Assets Become Programmable Resources**

 自动化、动态伸缩
* **Global, Available, and Unlimited Capacity**

* **Higher Level Managed Services**

 减少客户对底层基础设施的管理工作

* **Security Built In**
 
 云中的安全，在安全与合规性章节中做简单介绍。
 

> ### **云架构设计原则 **

AWS Cloud Architecting 最佳实践中提出了十个设计原则：

1. **扩展性 scalability**

2. **暴露资源而不是固定的服务器 Disposable Resources Instead of Fixed Servers**

3. **自动化 Automation**

4. **松耦合 Loose Coupling**

5. **服务，而不是服务器 Services, Not Servers**

6. **数据库 Databases**

7. **消除单点故障 Removing Single Points of Failure**

8. **成本优化 Optimize for Cost**

9. **缓存 Caching**

10. **安全 Security**

本章节对这十个最佳实践进行简单描述。

#### 扩展性

 * 纵向扩展
  
  例如单个 EC2 instance 的 CPU、内存、磁盘等的增加。
 
 * 横向扩展
 
  需要考虑以下几种情况：无状态应用、无状态组件、有状态组件、分布式处理（如大数据场景）。

#### 暴露资源而不是固定的服务器

* Instantiating Compute Resources

 对于实例化的计算资源，应该将资源创建过程自动化、模板化。AWS 通过以下几种方来实现：

 * Bootstrapping：引导脚本

 * Golden Images：经过验证的 image

 * Elastic Beanstalk：image + bootstrap 的混合模式

* Infrastructure as Code

 资源是可编程的，通过工具/技术/最佳实践实现基础设施的可重用 ( reusable), 可维护 (maintainable), 可扩展 (extensible), 和可测试 (testable)。

 AWS CloudFormation 可以实现 Infrastructure as Code，通过 CloudFormation 模板可定义一组 AWS 资源的组合，方便部署、升级、版本管理。
 
#### 自动化 Automation

 AWS 通过以下产品和服务来实现自动化
 AWS Elastic Beanstalk

	Amazon EC2 Auto recovery

		借助CloudWatch

	Auto Scaling

	Amazon CloudWatch Alarms

		可发消息至 Amazon Simple Notification Service（SNS），消息可触发一些操作

	Amazon CloudWatch Events

		可制定rule将event路由给其他服务做后续处理：Lambda functions,  Kinesis treams, SNS topics

	AWS OpsWorks Lifecycle event

		实现整个生命周期中环境的自动化的持续配置管理

	AWS Lambda Scheduled events

		通过事件驱动Lambda服务（serverless计算服务）
