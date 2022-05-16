# Learning Memo

## Docker
- Writing dockerfile
	- `FROM` creates a layer from the ubuntu:18.04 Docker image 
	- `COPY` adds files from your Docker client’s current directory.
	- `RUN` builds your application with make.
	- `CMD` specifies what command to run within the container. 
- Building docker image
	- `docker build -t {image name}:{tag} {the directry holding dockerfile}`
	- e.g., `docker build -t build2022/app:latest ${pwd}\python`
