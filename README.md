## 使用docker-compose进行代码部署
### 1

chitchat是《Go Web编程／ （新加坡）郑兆雄著 ， 黄健宏译》进行了改写的项目，可以进行创建帖子。

### 2

ghosttest 是慕[课网课](https://www.imooc.com/learn/867)程上的一个项目，利用了nginx，ghost,mysql进行组合实现的博客系统项目。

### 3 

docker-chitchat 是对chitchat项目进行了docker-compose部署，实现了两个容器。

编写了Dockerfile文件，docker-compose.yaml文件。将本地文件夹data挂载到postgres的数据库文件夹中。

这里有一个问题就是通过chitchat docker访问postgres docker时，无法通过localhost访问，只能查看psql的ip，然后进行改写，但是这个ip也不固定，这里host=172.17.0.2。本地可以通过localhost进行访问，不知道有没有大神可以提供方案。

