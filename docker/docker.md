
## 将docker镜像上传到本地其他仓库

docker pull oldImage

docker tag oldImage newImage

docker push newImage

## docker 批量删除镜像

docker rmi `docker ps | grep name`

批量删除Exited镜像
docker rm $(docker ps -a | grep Exited | awk '{print $1}')

## overlay2空间
/var/lib/docker/overlay2 目录会越来越大
通过docker system df 查看占用 删除无用镜像

删除无用镜像

