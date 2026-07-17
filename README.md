# zookeeper

版本：3.6\
下载镜像：docker pull zookeeper:3.6

```bash
windows系统
创建容器：
docker run --name zookeeper --publish 2181:2181 -d zookeeper:3.6 

# 进入zk客户端
docker exec -it zookeeper bash
zkCli.sh

启动容器：
docker start zookeeper

centeros系统：
docker pull wurstmeister/zookeeper  
docker run -d --log-driver json-file --log-opt max-size=100m --log-opt max-file=2  --name zookeeper -p 2181:2181 -v /etc/localtime:/etc/localtime wurstmeister/zookeeper  

```