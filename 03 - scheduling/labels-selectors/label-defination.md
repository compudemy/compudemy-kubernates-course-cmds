Get Pods, filteringg by selector

```bash
    kubectl get pods --selector app=app-1
```

Get Count of pods

```bash
    kubectl get pods | wc -l
```

The problem with the above command is that it outputs even the header label in the count

to solve this we use the no-headers option

```bash
    kubectl get pods --no-headers
```

And then we can do a word count on that

```bash
    kubectl get pods --no-headers | wc -l
```

Get Pods in multiple environments

```bash
    kubectl get pods --selector labe1=label-item,label2=label-item
```

