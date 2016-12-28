> ### **Auto Scaling**


使用 Auto Scaling，可以维持应用程序可用性，并且根据自定义的条件自动扩缩 Amazon EC2 的容量。可以使用 Auto Scaling 帮助确保运行所需数量的 Amazon EC2 实例。

在需求高峰期时，Auto Scaling 可以自动增加 Amazon EC2 实例的数量，以保证性能不受影响，当需求较低时，则会减少容量以降低成本。

Auto Scaling 既适合需求稳定的应用程序，同时也适合每小时、每天、每周使用量不停波动的应用程序。 


#### Auto Scaling 特性


* ##### 维持 Amazon EC2 实例的可用性

 不论运行多少个 Amazon EC2 实例，都可以使用 Auto Scaling 来检测有问题的 Amazon EC2 实例和运行状况不佳的应用程序，而且不用手工介入就能完成实例的替换工作。这样可确保应用程序获得预期的计算容量。 

* ##### 自动扩展 Amazon EC2 实例组合

 Auto Scaling 让客户能够密切跟踪应用程序的需求曲线，减少提前手动配置 Amazon EC2 容量的需求。

 例如，可以设置一个条件，当 Amazon EC2 实例组合的平均使用率较高时，就向 Auto Scaling 组添加新的 Amazon EC2 实例；同样，也可以设置一个条件，在 CPU 使用率较低时，以同样的增量删除实例。

 如果负载变化情况是可以预先判定的，则可以通过 Auto Scaling 设置一个计划，来对应用程序的扩展活动进行规划。可以使用 Amazon CloudWatch 发送警报，以触发扩展活动和 Elastic Load Balancing，帮助向 Auto Scaling 组中的实例分发流量。Auto Scaling 让客户能够以最佳使用率运行 Amazon EC2 实例组合。