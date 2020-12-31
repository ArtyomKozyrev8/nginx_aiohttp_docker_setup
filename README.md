# nginx_aiohttp_docker_setup
Example how to setup nginx in container to use it with separate aiohttp app in another container. 
The setup do not use Node frontend like React, otherwise setup should be made another way.


docker run --network=aio_net --name aio_ng -d -p 9999:80 aio_ng