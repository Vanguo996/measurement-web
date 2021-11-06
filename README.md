
react作为前端应用访问go server

部署kubesphere

```
https://github.com/kubesphere/ks-installer/releases/tag/v3.2.0 下载如下文件

kubectl apply -f kubesphere-installer.yaml

kubectl apply -f cluster-configuration.yaml

```


```
kubectl logs -n kubesphere-system $(kubectl get pod -n kubesphere-system -l app=ks-install -o jsonpath='{.items[0].metadata.name}') -f

kubectl get svc/ks-console -n kubesphere-system
```


