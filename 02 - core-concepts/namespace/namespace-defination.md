get All namespace

```bash
  kubectl get namespace
```

get All Pods in a namespace

```bash
  kubectl get pods
```

get All Pods in another namespace

```bash
  kubectl get pods --namespace=kube-system
```

Create a pod in another namespace

```bash
  kubectl get pods -n kube-pubic
```

or

```bash
  kubectl get pods --namespace=kube-pubic
```

Delete a pod in another namespace

```bash
  kubectl delete pod <pod-name> --namespace=kube-pubic
```




