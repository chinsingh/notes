# Managing [[Containerized App]]s in [[Docker]]

## Running a containerized app

```docker
docker container run -d --name containerName -p 8000:8080 \
>DockerHubID/repoName:imageName
```

### Flags

- `-d` **(detached)**: to run the container in the background detached from the terminal
- `--name` : to specify the container name
- `-p` : for [[Port Mapping or Forwarding]] — any request to port 8000 on your system/remote server will redirect to port 8080 of the container - where the app is running.
- `-it` (interactive terminal): to run the container in foreground attached to the terminal
  - In this mode, you can run any command in your terminal and it will actually get executed on the container. You will be basically be inside the container on your terminal.
  - You can come out of it using `exit` command. Although, this will also kill the container, as you are effectively killing the shell process that was the main process of the container.
  - Leaving the container without terminating it: Ctrl + P + Q

### How docker gets the image

- Docker first checks locally for the container image. If it doesn’t exist, then it goes to the Docker hub
- If you want to run image from a different registry, you need to enter the URL of the image.

### Running

- On local system — localhost:8000
- On cloud system — DNS/public IP of the cloud instance:8000

## Managing a containerized app

### Stopping the app

```docker
docker container stop containerName
```

Docker sends the app a [[SIGTERM]] signal and waits for a few seconds for it to shut down gracefully. If it doesn’t, its terminated with a [[SIGKILL]]

### Starting the app

```docker
docker container start containerName
```

### Removing the app

```docker
docker container rm containerName
```

#### Removing the app forcefully

`-f` flag

## Listing containers

### Listing running containers

```docker
docker container ls
```

### Listing all images/containers

Use a `-a` flag along with the command.
