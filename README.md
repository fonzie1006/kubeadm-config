kubeadm 初始化kubernetes集群所需要的配置，根据我自己的需求修改的配置文件。有一些(你懂的)网络访问问题,这里默认镜像仓库用的是阿里云的，根据需求可以更改.

#### 版本适用说明

目前可以适用于kubernetes v.1.13.x+ 版本的配置

[kubeadm-init.yaml](https://github.com/fonzie1006/kubeadm-config/blob/master/kubeadm/cluster-manager/kubeadm-init.yaml)的网络是flannel的，如果要使用其他网络请自行修改.

#### 目录说明

* [docker/config/damon.json](https://github.com/fonzie1006/kubeadm-config/blob/master/docker/config/daemon.json) : 存储```/etc/docker/daemon.json```的配置文件
* [kubeadm/cluster-manager/kubeadm-init.yaml](https://github.com/fonzie1006/kubeadm-config/blob/master/kubeadm/cluster-manager/kubeadm-init.yaml): master节点初始化的配置文件
* [kubeadm/cluster-manager/kubeadm-join.yaml](https://github.com/fonzie1006/kubeadm-config/blob/master/kubeadm/cluster-manager/kubeadm-join.yaml): node节点加入kubernetes集群的配置


#### 配置模版说明

在YAML配置文件中 ```<xxx>```是需要自己替换
