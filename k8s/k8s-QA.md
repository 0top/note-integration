k8s:
Q: 不同namespace直接如何通过相互访问
A: 可以通过service, service-name.namespace当做域名访问即可
    kubectl get svc -n namespace
    
Q: 相同namespace下如何项目访问
A: 通过service-name.namespace即可，可以在pod中/etc/resolve.conf中查看

Q: pod访问机制
A: pod首先寻找service中路由，如果没找到，则去宿主机中寻找，若宿主机可访问则pod也可

Q: 如何将pod固定在某些node上
A: 通过给node设置label,在部署pod时候可以通过nodeSelector将pod指定到包含对应label的机器上


