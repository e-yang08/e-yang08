# Learning Memo

## Docker
- Writing dockerfile
	- `FROM` creates a layer from the ubuntu:18.04 Docker image 
	- `COPY`: copies files from a source location in local to a destination in the Docker container
		- e.g., `COPY <src> <dest>` 
	- `RUN` builds your application with make.
	- `CMD`: commands to run within the container. can be overwritten unlike `ENTRYPOINT`
		- e.g., `CMD ["executable", "parameter 1", "parameter 2"...]` 
		- `CMD [""]` -- parameters to entrypoint
	- `WORKDIR`: change the working directory inside the container but not the source 
- Building docker image
	- `docker build -t {image name}:{tag} {the directry holding dockerfile}`
	- e.g., `docker build -t build2022/app:latest ${pwd}\python`
