# OpenStack产品体系

OpenStack 是项目（Project）驱动的，参见 OpenStack 官方网站里对项目的描述。

* **6 个核心项目和 13 个可选项目**

 http://www.openstack.org/software/project-navigator

* **所有项目列表**

 https://governance.openstack.org/tc/reference/projects/index.html 


需要关注几个点：

* 项目成熟度指标和重点项目的成熟度情况

* OpenStack 各服务设计和架构的一些通用思想，比如各服务的 api 组件（如 nova-api、neutron-server、cinder-api 等等）、plugin 与 driver 框架（如 nova-compute 对多 hypervisor 的支持、cinder-volume 对多存储后端的支持等） 

* 对重点项目的深入理解（UOS 201 内容）

* 几大核心项目之间的交互流程（UOS 201 内容）

![](/assets/mainservice.png)



