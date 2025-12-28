# hub-docker-demo

show how to build a docker image and push it to hub.docker.com.


you should make a settings of secrets:
- DOCKER_HUB_USERNAME
- DOCKER_HUB_TOKEN

```shell
        # git tag v1.2.3
        # git push origin v1.2.3
```

## refer

docker login -u <hub.docker.com账号>    之后输入密码

docker build -t test:v0.0.1 . 
docker tag test:v0.0.1 <hub.docker.com账号>/test:v0.0.1

or 
docker build -t <hub.docker.com账号>/test:v0.0.1 .

> <hub.docker.com账号>/test 指 <hub.docker.com账号>/仓库名，在https://hub.docker.com/repositories/<hub.docker.com账号>中可以看到。


docker push <hub.docker.com账号>/test:v0.0.1


