apiVersion: v1
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
