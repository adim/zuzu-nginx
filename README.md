# Run docker locally

Build docker image:
docker build -t some-content-nginx . 
Run it:
docker run --name some-nginx -d -p 8080:80 some-content-nginx

connect via bash to the container:
docker exec -it some-nginx /bin/bash

check content of root directory:
curl -X GET   http://localhost:8080 