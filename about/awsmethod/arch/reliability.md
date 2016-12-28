> ### **Reliability Pillar**

#### 设计原则


1. **Test recovery procedures**

2. **Automatically recover from failure**

3. **Scale horizontally to increase aggregate system availability**

4. **Stop guessing capacity**

5. **Manage change in automation**


#### 定义和实现

1. **Foundations**

 管理 AWS service list

 IAM、VPC，合理规划架构、网络拓扑

2. **Change management**

 变更管理、如何执行变更（参见 [ITIL Asset and Configuration Management in the Cloud](https://d0.awsstatic.com/whitepapers/AWS_Asset_Config_Management.pdf) 白皮书）

 CloudWatch：监控资源使用情况

 CloudTrail：记录 API call 的 log 供审计

3. **Failure management**

 备份数据

 可靠性测试、灾难恢复规划

 CloudFormation：预定义好执行模板（使行为可预测）