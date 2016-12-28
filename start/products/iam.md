> ### **AWS Identity and Access Management**


AWS Identity and Access Management (IAM) 使企业能够安全地控制用户对 Amazon AWS 服务和资源的访问权限。企业可以使用 IAM 创建和管理 AWS 用户和群组，并使用各种权限来允许或拒绝他们对 AWS 资源的访问。 

IAM 是 AWS 账户提供的一项功能，不另外收费。只需为企业的用户所用的其他 AWS 服务付费。

#### AWS Identity and Access Management 功能

* ##### 管理 IAM 用户及其访问权限

 可以在 IAM 中创建用户，为其分配单独的安全凭证（或称为访问密钥、密码、多重验证设备）或请求临时安全凭证，供用户访问 AWS 服务和资源。可以管理权限，以控制用户可以执行哪些操作。

* ##### 管理 IAM 角色及其权限 

 可以在 IAM 中创建角色并管理权限，以便控制承担该角色的实体或 AWS 服务可以执行哪些操作。也可以定义由哪个实体承担该角色。

* ##### 管理联合身份用户及其权限

 可以启用联合身份功能，以允许公司中的现有身份（用户、组和角色）访问 AWS 管理控制台、调用 AWS API 并访问资源，而无需为各个身份创建 IAM 用户。

#### AWS Identity and Access Management 最佳实践

* 用户 – 创建单独的用户。

* 组 – 利用组来管理权限。

* 权限 – 授予最低权限。

* 审核 – 打开 AWS CloudTrail。

* 密码 – 配置强大的密码策略。

* MFA – 为特权用户启用 MFA（AWS Multi-Factor Authentication，多因子认证）。

* 角色 – 将 IAM 角色用于 Amazon EC2 实例。

* 共享 – 使用 IAM 角色共享访问权限。

* 轮换 – 定期轮换安全凭证。

* 条件 – 利用条件进一步限制特权访问。

* 根 – 减少或删除根的使用。

