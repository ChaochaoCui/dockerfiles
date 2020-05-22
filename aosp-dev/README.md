https://github.com/shugaoye/docker-aosp 

docker run -it -e USER_ID=$(id -u) -e GROUP_ID=$(id -g) -v /local_path/:/docker_path:rw aosp-dev:v0 bash
