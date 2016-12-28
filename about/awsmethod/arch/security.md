> ### **Security Pillar**

#### 设计原则


1. **Apply security at all layers**

2. **Enable traceability**
 
  log & audit

3. **Implement a principle of least privilege**

4. **Focus on securing your system**
 
 AWS shared responsibility model 共同责任模型
 https://aws.amazon.com/compliance/shared-responsibility-model/
 
 ![](/assets/共同责任安全模型.JPG)

5. **Automate security best practices**

 基于软件的安全机制


#### 定义和实现

1. **Identity and access management**

 IAM：Identity and Access Management

 MFA：multi-factor authentication

2. **Detective controls**

 logs, events and monitoring

3. **Infrastructure protection**

 MFA、AMI、配置管理等

 VPC

4. **Data protection**

 数据分类分级、加密、操作日志、副本

 KMS： Key Management Service

 SSE：Server Side Encryption（for S3）

5. **Incident response**

 log、event（出现问题时的自动化脚本）

 CloudFormation（预执行工具）

