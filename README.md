```
Name:              intolerable-nginx-service
Namespace:         default
Labels:            app=nginx
Annotations:       kubectl.kubernetes.io/last-applied-configuration:
                     {"apiVersion":"v1","kind":"Service","metadata":{"annotations":{},"labels":{"app":"nginx"},"name":"intolerable-nginx-service","namespace":"...
Selector:          app=nginx
Type:              ClusterIP
IP:                10.97.88.56
Port:              <unset>  80/TCP
TargetPort:        80/TCP
Endpoints:
Session Affinity:  None
Events:            <none>
(⎈ |kafka:default) tolerate-test kubectl describe service nginx-service
Alias tip: k describe service nginx-service
Name:              nginx-service
Namespace:         default
Labels:            app=nginx
Annotations:       kubectl.kubernetes.io/last-applied-configuration:
                     {"apiVersion":"v1","kind":"Service","metadata":{"annotations":{},"labels":{"app":"nginx"},"name":"nginx-service","namespace":"default"},"s...
Selector:          app=nginx
Type:              ClusterIP
IP:                10.106.199.5
Port:              <unset>  80/TCP
TargetPort:        80/TCP
Endpoints:         172.17.0.16:80,172.17.0.17:80,172.17.0.18:80
Session Affinity:  None
Events:            <none>
(⎈ |kafka:default) tolerate-test kubectl get pod -l app=nginx
NAME                                READY   STATUS    RESTARTS   AGE
nginx-deployment-7f85f44fcf-n6k6b   0/1     Running   0          4m9s
nginx-deployment-7f85f44fcf-nmz8k   0/1     Running   0          4m9s
nginx-deployment-7f85f44fcf-ztsn9   0/1     Running   0          4m9s
```
