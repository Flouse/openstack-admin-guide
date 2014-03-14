Get started with OpenStack
==========================

OpenStack项目是一个开源云计算平台，该项目的宗旨是易于使用，高度可扩展，功能丰富，它是由来自世界各地的开发者和云计算专家共同创建的。OpenStack通过一系列相互关联的服务提供了一个基础设施即服务(IaaS)的解决方案。
每一个服务提供API用来和其他服务进行交互集成，根据你的需求，你可以选择性的安装其中一些服务。

下表简单的描述了组成OpenStack的各个服务：

==================      ==============                ==================
Service                 Project Name                  Description
==================      ==============                ==================
Dashboard               Horizon                       提供了一个基于web的控制面板，和底层的各个OpenStack服务进行交互，比如创建虚拟机实例，分配IP地址，控制访问权限等。
Compute                 Nova                          管理虚拟机实例(instance)的整个生命周期，主要负责根据需求来创建，调度，销毁虚拟机实例。
Networking              Neutron
ObjectStorage           Swift
BlockStorage            Cinder
Identity Service        Keystone
Image Service           Glance
Telemetry               Ceilometer
Orchestration           Heat
==================      ==============                ==================

.. toctree::
   :maxdepth: 2

   conceptual_architecture
   services/index
