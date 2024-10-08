docker images
docker ps 
docker ps -a 
docker rm <容器id>
docker rmi <镜像id>
docker restart <容器id>
docker stop <容器id>

systemctl enable docker # 开机启动
service docker stop # 关闭docker

docker pull
docker exec -it <容器名> bash
docker cp <容器名>: /sourcePath /targetPath # 拷贝文件

linux 命令

whereis  <服务名>

service mysqld status