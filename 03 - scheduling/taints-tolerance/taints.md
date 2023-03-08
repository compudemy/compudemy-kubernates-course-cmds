to taint a node we use the following commands

```bash
    kubectl taint nodes node1<node-name> app=blue:Noschedule
```

To check the taint on a node

```bash
    kubectl describe node <node-name> | grep Taint
```

to generate a yaml file from an imperative cmd

```bash
    kubectl run bee --image=nginx --dry-run=client -o yaml > bee.yaml
```


```bash
    tolerations:
    - key: "key1"
    operator: "Equal"
    value: "value1"
    effect: "NoSchedule"

```