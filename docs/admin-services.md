# Start or Stop the Services

These commands you must know when you using the JupyterLab of Websoft9

## JupyterLab

```shell
sudo systemctl start jupyterlab-server
sudo systemctl stop jupyterlab-server
sudo systemctl restart jupyterlab-server
sudo systemctl status jupyterlab-server

# you can use this debug mode if JupyterLab service can't run
jupyterlab-server console
```

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