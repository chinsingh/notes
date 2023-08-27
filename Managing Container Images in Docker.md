# Managing [[Container Image]]s in [[Docker]]

## Building an image

```docker
docker image build -t yourDockerHubID/repoName:imageName
```

## Hosting image on [[Container Registr]]y

```docker
docker image push yourDockerHubID/repoName:imageName
```

## Listing local images

```docker
docker image ls
```
