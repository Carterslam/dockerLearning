深度剖析kubernates

06.白话容器基础（二）：隔离与限制
Cgroups的作用，是限制单个进程（容器）占用宿主机的资源上限
$ docker run -it --cpu-period=100000 --cpu-quota=20000 ubuntu /bin/bash （该容器最大占用20%cpu资源）

07 | 白话容器基础（三）：深入理解容器镜像
Docker容器内部默认继承宿主机的文件夹，可重新挂在（mount namesapace）

Linux 容器的核心实现原理：Linux Namespace 的隔离能力、Linux Cgroups 的限制能力 基于 rootfs 的文件系统
