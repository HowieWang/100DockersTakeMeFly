# 100DockersTakeMeFly
Love playing with Docker, and believe 100 Dockers will Take Me Fly!

> You can check details in every folder.

- [ ] 1-webide
- [ ] 2-nginx





## 时速云操作指南

    * 下载镜像 
    在本地 docker 环境中输入以下命令，就可以pull一个镜像到本地了。

    sudo docker pull index.tenxcloud.com/<namespace>/<repository>:<tag>
    注意：为了在本地方便使用，下载后您可以修改tag成短标签，比如

    sudo docker tag index.tenxcloud.com/mysql:latst mysql:latest
    * 发布镜像
    1. 在本地 docker 环境中输入以下命令进行登录。

    sudo docker login index.tenxcloud.com
    2. 假如在本地已经有了想要push的image,比,如这个image名为hello-world。如果在本地没有image,可以首先从Docker官方网站去pull一个下来。

    docker pull hello-world:latest
    3. 然后，需要对这个image进行标记，在命令中输入：

    sudo docker tag hello-world:latest index.tenxcloud.com/username/hello:latest(自定义仓库名);
    4. 最后在命令行输入如下命令就可以push这个image到你创建的镜像仓库中了。

    sudo docker push index.tenxcloud.com/username/hello:latest(自定义仓库名).









----
##reference:  

- https://help.github.com/articles/writing-on-github/
