# Docker Documentation
Building and pushing updated versions of the API

docker build . -t yourDockerTagName/restaurant-api:latest
- this is to build a new api version --> you need the :tagname at the end
- here tagname is latest

docker push yourDockerTagName/restaurant-api:latest
- after you build it, push it

sudo docker pull yourDockerTagName/restaurant-api:latest 
- this is done in powershell, pulling it down onto our server

sudo docker run -d -p 3000:3000 yourDockerTagName/restaurant-api:latest
- to start the image(s)
- we are running it on port 3000 (-p 3000:3000)

sudo docker stop $(docker ps -a -q)
- stop the image(s) from running
