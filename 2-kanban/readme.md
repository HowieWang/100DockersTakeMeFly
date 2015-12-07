docker run -d --name kanban \
    -v /kanban/data:/var/www/html/data \
    -v /kanban/assets:/var/www/html/assets \
    -P  mkodockx/docker-kanban