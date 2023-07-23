# 香菜饅頭營
## Use `curl` in a pod to list all pods in namespace `default`

### How to
```bash
kubectl apply -f curl.yaml && kubectl wait --for=condition=complete job/curl-list-pod-job --timeout=30s && kubectl logs job/curl-list-pod-job && kubectl delete job/curl-list-pod-job
```

The above command will create resources for using curl listing pods in a pod, show the result and clean up.
