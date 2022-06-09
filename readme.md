Build Image -- Run the command in terminal
docker build -t [IMAGE_NAME] .
e.g. docker build -t myapp2 .

Build Image with a tag -- Run the command in terminal
docker build -t [IMAGE_NAME]:[TAG] .
e.g. docker build -t myapp2:v1 .

Start up Docker ---- Run the command in terminal
docker run --name [CONTAINER_NAME] -p [LOCAL_PORT]:[DOCKER_PORT] -d [IMAGE_NAME]
e.g. docker run --name myapp_c2 -p 4000:4000 -d myapp

View All Container ---- Run the command in terminal
docker ps -a

Start A Container ---- Run the command in terminal
docker start [CONTAINER_NAME]
e.g. docker start myapp_c3

Stop A Container ---- Run the command in terminal
docker stop [CONTAINER_NAME]
e.g. docker stop myapp_c3

View All Images ---- Run the command in terminal
docker images

Remove An Image ---- Run the command in terminal
docker images rm [IMAGE_NAME]
e.g. docker images rm myapp

Remove A Container ---- Run the command in terminal
docker container rm [CONTAINER_NAME]
e.g. docker container rm myapp_c3

Remove An Image which is USE status --- Run the command in terminal
docker images rm [IMAGE_NAME] -f

Delete all Images and Volumes ---- Run the command in terminal
docker system prune -a