# CTFd v3.6.0 + ctfd-whale + ctfd-pages-theme


## 注意事项
- ！！！！ 不要clone
- 请在 Releases 栏下载最新集成修改版本！！
- 




## Update

> v3.6.0
- 后台添加docker动态环境,增加docker images 列表
- 修复前台一些bug
- 添加了矩阵记分板

> v3.6.1
- 新增解题播报功能
- 提交正确的flag后，可以向其他在线用户播报（并添加到通知里，也可以修改不添加）
- 此修改版本遇到任何使用上的问题，可以联系我，群号在下面。

## 部分说明

* 集成环境

- CTFD version 3.6.0
- ctfd-whale  (docker 部署赛题)
- ctd-pages-theme (赛题分页显示)



- bilibili 视频使用教程

https://www.bilibili.com/video/BV1sK4y1w7uH

- 下载地址
https://github.com/imLZH1/ctfd_whale_pages






## Docker 安装



```python
sudo apt install docker
sudo apt install docker-compose
```





## 需要配置哪些？





* 端口范围



![image](image-20230920042250-cotz2cn.png)





* docker加速

```python
/etc/docker/daemon.json 

{
  "registry-mirrors": [
    "https://docker.mirrors.ustc.edu.cn"
  ]
}
```



## 初始化集群



```python
sudo docker swarm init
sudo docker node update --label-add='name=linux-1' $(sudo docker node ls -q)
```

![image](image-20230920042406-kbsxzt3.png)​





## CTFd ！启动



```pytthon
sudo docker-compose up -d
```

![image](image-20230920042620-jes8gsf.png)​



## 打包好的



```python
git clone https://github.com/imLZH1/ctfd_whale_pages.git
cd ctfd_whale_pages
docker-compose up -d

```



启动好后 用 admin:admin 登录后台 config->reset 清除数据，然后你就可以自己配置啦·？



* 交流群

```python

蔡徐坤篮球协会 信息部
QQ: 591613671
```

