```apiVersion: v1
kind: Pod
metadata:
  creationTimestamp: null
  labels:
    run: minisite
  name: minisite
spec:
  containers:
  - image: shollynoob/minisite
    name: minisite
    resources: {}
  dnsPolicy: ClusterFirst
  restartPolicy: Always
status: {}
```



###Describe pod

```Name:             minisite
Namespace:        default
Priority:         0
Service Account:  default
Node:             gke-miniproject-default-pool-aa9e3dcd-3gsv/10.128.0.6
Start Time:       Sun, 05 Mar 2023 22:37:18 +0000
Labels:           run=minisite
Annotations:      <none>
Status:           Running
IP:               10.84.0.6
IPs:
  IP:  10.84.0.6
Containers:
  minisite:
    Container ID:   containerd://fa1a5eba4eae621350efdaad1e3dcbf0743d2cff962b29a28957b1afe133eb59
    Image:          shollynoob/minisite
    Image ID:       docker.io/shollynoob/minisite@sha256:92e46e040598c72f5a25e178852268ab5b3479d2449c8f37dad6ab12507aec5b
    Port:           <none>
    Host Port:      <none>
    State:          Running
      Started:      Sun, 05 Mar 2023 22:37:22 +0000
    Ready:          True
    Restart Count:  0
    Environment:    <none>
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-jql76 (ro)
Conditions:
  Type              Status
  Initialized       True
  Ready             True
  ContainersReady   True
  PodScheduled      True
Volumes:
  kube-api-access-jql76:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type    Reason     Age    From               Message
  ----    ------     ----   ----               -------
  Normal  Scheduled  4m52s  default-scheduler  Successfully assigned default/minisite to gke-miniproject-default-pool-aa9e3dcd-3gsv
  Normal  Pulling    4m51s  kubelet            Pulling image "shollynoob/minisite"
  Normal  Pulled     4m48s  kubelet            Successfully pulled image "shollynoob/minisite" in 2.644540092s
  Normal  Created    4m48s  kubelet            Created container minisite
  Normal  Started    4m48s  kubelet            Started container minisite```
