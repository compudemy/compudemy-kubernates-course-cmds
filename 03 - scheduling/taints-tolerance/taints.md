to taint a node we use the following commands

```bash
    kubectl taint nodes node1<node-name> app=blue:Noschedule
```

To check the taint on a node

```bash
    kubectl describe node <node-name> | grep Taint
```