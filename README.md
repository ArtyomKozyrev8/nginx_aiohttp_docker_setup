# nginx_aiohttp_docker_setup
Example how to setup Nginx in container to use it with separate aiohttp app in another container. 
The setup do not use Node frontend like React, otherwise setup should be made another way.

**How to get repository:**

git clone https://github.com/ArtyomKozyrev8/nginx_aiohttp_docker_setup.git

**How to run and build container:**

docker build -t aio_ng .

docker run --network=aio_net -v aio_serv_v:/static -v aio_serv_v2:/static2 --name aio_ng -d -p 8585:80 aio_ng