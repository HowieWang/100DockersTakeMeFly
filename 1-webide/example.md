
创建工作文件夹：

    mkdir mywork

进入目录

    cd mywork

启动docker，注意这里是大写-P，如果自定义端口请注意容器里面端口为`->22/tcp和->8181/tcp`

    # docker run -it --name myname -d -P -v $(pwd):/cloud9/workspace agungf/cloud9-ide

这里就会启动一个默认端口的cloud9-ide啦！

    # docker ps
    CONTAINER ID        IMAGE                                           COMMAND                CREATED             STATUS              PORTS                                            NAMES
    9d7b56f7e097        agungf/cloud9-ide                               "/bin/sh -c /usr/bin   5 seconds ago       Up 4 seconds        0.0.0.0:32783->22/tcp, 0.0.0.0:32782->8181/tcp   myname   