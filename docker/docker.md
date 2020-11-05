
## 将docker镜像上传到本地其他仓库

docker pull oldImage

docker tag oldImage newImage

docker push newImage

## docker 批量删除镜像

docker rmi `docker ps | grep name`



