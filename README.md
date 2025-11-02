

## Docker

```shell
docker run -d -p 25501:25501 --restart always --name subweb careywong/subweb:latest
```

若需要对代码进行修改，你需要在本地构建镜像并运行。
注：每次修改代码，你都需要重新执行 docker build 来执行打包操作。

```shell
docker -v
Docker version 23.0.4, build f480fb1

docker build -t subweb-local:latest .
docker run -d -p 25501:25501 --restart always --name subweb subweb-local:latest
```
