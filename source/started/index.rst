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
Networking              Neutron                       为OpenStack的其他服务提供网络连接服务，并且提供API给用户来自定义网络，由于它可插拔的架构，可以支持很多流行的网络技术。
ObjectStorage           Swift                         通过RESTful接口存取任意的非结构化数据对象。由于它的数据复制和可扩展性，具有高度容错性。它的实现并不像挂载了很多文件目录的文件服务器一样。
BlockStorage            Cinder                        为虚拟机提供持久化块存储服务，它可插拔的架构使得管理块存储设备变的很方便。
Identity Service        Keystone                      为其他的OpenStack服务提供认证和授权服务，并且提供所有OpenStack服务的endpoints
Image Service           Glance                        存取镜像，创建虚拟机的过程中，会使用到它
Telemetry               Ceilometer                    监控和计量整个OpenStack云平台，可以用来计费，基准检测，扩展和数据分析
Orchestration           Heat                          用OpenStack自己定义的HOT模板或者是AWS的CloudFormation模板来协调组织多个混合的云应用程序，实现了OpenStack自己定义的RESTful API和兼容AWS CloudFormation的API
==================      ==============                ==================

.. toctree::
   :maxdepth: 2

   conceptual_architecture
   logical_architecture
   services/index
