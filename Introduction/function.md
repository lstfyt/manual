# 1.2 主要功能
Mevoco产品是私有云管控系统，提供了对用户数据中心的计算、存储、网络等资源的管理和调度。用户使用Mevoco产品可以快速的配置私有云环境，并通过Mevoco快速的创建云主机、分配云盘和自动配置云主机网络。

Mevoco的具体功能包括：

|组件|功能|
| --- | --- |
| 物理机 | 支持KVM虚拟化、支持嵌套虚拟化、支持本地高速存储; - 支持操作：新增、删除、维护、监控、启用、停用、重连等 |
| 云主机 | 支持Windows (支持Virtio驱动)、Linux等主流操作系统;支持操作：创建、批量创建、停止、启动、控制台、删除、恢复、彻底删除、设置静态IP地址、挂载云盘、卸载云盘、挂载ISO、卸载ISO、调整启动顺序、创建镜像、迁移、监控、创建快照、恢复快照、高可用、更改所有者、指定物理机启动等 ; 支持设置不同的云主机模板; 支持设置云主机的磁盘IO的上限和网络IO的上下限; 自动探测更新云主机状态变化 |
| CPU | 支持资源超分配 |
| 内存 | 支持资源超分配 |
| 云盘 | 支持qcow2和raw两种格式操作：支持挂载、卸载、创建快照、恢复快照等操作 |
| 网络 | 支持多网络、分布式DHCP、分布式EIP、AWS SSH key注入 |
| 安全组 | 支持IP层网络隔离，包括添加防火墙规则和设定需要进入防火墙的云主机 |
| 弹性IP | 支持公有网络访问私有网络 |
| 存储 | 支持本地存储、NFS、Ceph、Shared Mount Point等类型。支持资源超分配、支持资源监控、资源分配上限阈值 |
| 镜像服务器 | 支持Ceph或网络存储、支持云主机镜像、支持ISO（光盘）镜像、支持添加多台镜像服务器 |
| 用户管理 | 支持账户、用户组、用户三种粒度的资源权限控制 |
| 计费 | 支持对CPU、内存、云盘资源以时长对不同账户进行计费 |
| 设置 | 支持设置管理员密码、资源删除策略、会话登录超时、CPU模式、高可用、CPU超分、云主机磁盘缓存模式等 |
| 性能监控 | 支持对物理机、云主机的CPU、内存、存储、网络等使用情况按照指定时间间隔统计分析 |
