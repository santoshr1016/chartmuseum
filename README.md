### How to run

## This is very simple helm chart,
```text
Chart name should be same as the directory in which it resides

helm ls
helm install --name XXX .
helm delete --purge XXX
helm upgrade XXX .
helm rollback XXX 1
helm upgrade XXX . --set service.type=NodePort
```

### How to Host charts in github
```text
1. Create a new hithub repo with default README.md (optional)
2. Get your chart folder.
3. Package it using the command 
    # helm package CHART_FOLDER
4. Create the index.html
    # helm repo index .
5. git add.
6. git push

```
