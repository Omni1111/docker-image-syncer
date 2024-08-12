# docker-image-syncer

## 简介
1. auth.json 认证信息配置文件
2. image.json 单镜像同步规则配置文件
3. images.json 多镜像同步规则配置文件

## 使用

### 申请容器镜像服务 ACR
配置 命名空间，需要的仓库，访问凭证的密码

### 设置用户名、密码、命名空间
Setting -> Secrets and Variables -> Action 
添加 Repository secrets
1. ACR_PASSWORD
2. ACR_USERNAME
3. NAMESPACE

## Workflow
### 单镜像同步

Sync Single Image，填写源镜像，如：nginx:latest，目标镜像，如：（nginx:latest）或者自定义，需要提前添加仓库，其他可以默认或修改。

单镜像会同步已存在的镜像

### 多镜像同步

Sync Multiple Image，需要在images.json中编写对应的同步规则。



