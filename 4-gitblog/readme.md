docker pull index.tenxcloud.com/dockerxman/docker-gitblog 
mkdir gitblog
cd gitblog
vim welcome.md

write something....

----
然后运行下面的脚本。

sh gitblog.sh

    #!/bin/sh
    docker stop gitblog
    docker rm gitblog
    docker run -itd -p 1111:80 -v $(pwd):/www/gitblog-master/blog  --name gitblog index.tenxcloud.com/dockerxman/docker-gitblog
