# 服务启停

使用由Websoft9提供的 JupyterLab 部署方案，可能需要用到的服务如下：

## JupyterLab

```shell
sudo systemctl start jupyterlab-server
sudo systemctl stop jupyterlab-server
sudo systemctl restart jupyterlab-server
sudo systemctl status jupyterlab-server

# you can use this debug mode if JupyterLab service can't run
jupyterlab-server console
```

### MySQL

```shell
sudo systemctl start mysql
sudo systemctl stop mysql
sudo systemctl restart mysql
sudo systemctl status mysql
```

### Redis

```shell
systemctl start redis
systemctl stop redis
systemctl restart redis
systemctl status redis
```