# Ceph deployment for Kubernetes(Single Machine)

> [!CAUTION]
> Development and testing purposes only. Use at your own risk.

## Description
* Deploy rook v1.14.2, Ceph v18.2.2, CephFS to all worker nodes in a cluster.
* Use `/dev/sdb` as osd from each worker nodes.
* Disable node anti-affinity in CephFS provisioner configuration to allow deployment on a single-node cluster.

## Tested Environment
* Ubuntu Server 22.04 LTS, AMD64
* Containerd v1.6.31
* Kubernetes v1.28.9, Generic
* Cilium v1.15.4

Upstream source: [rook v1.14.2](https://github.com/rook/rook/tree/v1.14.2)
