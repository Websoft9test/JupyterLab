# jupyterlab on CentOS.notes

组件名称：jupyterlab
安装文档：https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html
配置文档：https://jupyter.readthedocs.io/en/latest/projects/content-projects.html#configuration
支持平台： Debian家族 | RHEL家族 | Windows 
gi
责任人：helin--

## 概要

- Jupyter 项目用于开发开放源码软件、开放标准和跨数十种编程语言的交互式计算服务

## 环境要求

- 程序语言：python
- 应用服务器：自带
- 数据库：无
- 依赖组件：无

## 安装说明

### 这里我们使用pip安装jupyterlab在centos上

```
pip install --upgrade pip           #更新pip
pip install jupyterlab          #安装jupyterlab
pip install notebook          #安装notebook
jupyter notebook              #运行notebook
pip install voila            #安装voila

```

### 或者使用docker安装jupyterlab在centos上

https://jupyter-docker-stacks.readthedocs.io/en/latest/

```
yum install docker  #安装docker
systemctl docker start   #启动docker
docker run -p 8888:8888 jupyter/scipy-notebook:17aba6048f44

```





## 配置

默认情况下，配置文件存储在目录中。`~/.jupyter`



## 服务

本项目安装后会自动生成

## 版本问题
sudo sh -c "echo jupyter-lab --version 1>> /data/logs/install_version.txt"

## 常见问题

#### 有没有管理控制台？

*http:// 公网 IP:8888  即可进入控制台 

![image-20200421180147138](C:\Users\w9\AppData\Roaming\Typora\typora-user-images\image-20200421180147138.png)

#### 本项目需要开启哪些端口？

| item         | port  |
| ------------ | ----- |
| 管理平台端口 | 8888  |
| 通讯端口     | 61616 |
| http         | 15672 |



## 日志

- 2020-04-22完成CentOS安装研究

问题：

1.OSError: [Errno 99] Cannot assign requested address

```
jupyter notebook --ip=0.0.0.0 --allow-root #使用此命令启动
```


