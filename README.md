# Run Nginx locally with Docker:

Build docker image:\
docker build -t some-content-nginx . 
# Run docker container:\
Run it: \
docker run --name some-nginx -d -p 8080:80 some-content-nginx 
# Run Nginx locally with Docker Compose:
connect via bash to the container: \
docker exec -it some-nginx /bin/bash 
# Run Nginx locally with Docker:
check content of root directory: \
curl -X GET   http://localhost:8080 