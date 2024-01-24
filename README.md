# devops-project1

# command to build docker image
docker build -t custom-web:v1 .

# command to run conatiner
docker run --name custom-web1 -d -p 8081:80 custom-web:v1

# command to stop current running conatiner
docker rm -f custom-web1

# command to remove docker image
docker image rm -f custom-web:v1