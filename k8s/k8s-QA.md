k8s:
Q: 不同namespace直接如何通过相互访问
A: 可以通过service, service-name.namespace当做域名访问即可
    kubectl get svc -n namespace
    
Q: 相同namespace下如何项目访问
A: 通过service-name.namespace即可，可以在pod中/etc/resolve.conf中查看

Q: 




