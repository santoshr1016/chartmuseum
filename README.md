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

### How to "host" charts in github
```text
0. Create a new github repo with default README.md (optional).
1. cd chartmuseum.
2. Copy your chart folder here.
3. Package it using the command. 
    # helm package CHART_FOLDER
    # helm package mynginx
    # it will create .gz file mynginx-0.3.0.tgz    
4. Create the index.html
    # helm repo index .
5. git add.
6. git push


```

### How to use charts from the new hosted github repo
```text
1. helm repo list
2. helm repo add mycharts https://raw.githubusercontent.com/santoshr1016/chartmuseum/master
3. helm repo list
4. helm install --name sasa mycharts/mynginx ( "mychart" is the local alias for the chartmuseum, see instruction 2 )
5. helm ls


```
