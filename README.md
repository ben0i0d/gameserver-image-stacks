# gameserver-image-stacks



## 我是谁
这是用于构建eoelab中游戏服务器镜像项目  
## 镜像依赖关系
节点内为镜像，默认子节点是父节点的派生  
base为Debian:bullseye
```mermaid
	graph LR
	A(base)-->B(Minecraft)
	B-->C(Java-8)
    B-->D(Java-17)
    A-->E(Steam)
```
