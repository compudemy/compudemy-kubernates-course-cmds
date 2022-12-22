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
  kubectl run nginx --image=nginx -n kube-pubic
```

or

```bash
  kubectl run nginx --image=nginx  --namespace=kube-pubic
```

Delete a pod in another namespace

```bash
  kubectl delete pod <pod-name> --namespace=kube-pubic
```

To create a namespace

```bash
  kubectl create -f <defination-file.yaml> --namespace=namespace
```

where namespace is where we want the resource created e.g dev or kube-pubic

To delete a namespace

```bash
  kubectl delete namespace dev
```

To set another namespace to default

```bash
  kubectl config set-context $(kubectl config current-context) --namespace=dev
```


