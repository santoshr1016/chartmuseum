### How to run

## Thi is very simple helm chart, Its not parametrized.
```text
Chart name should be same as the directory in which it resides

helm ls
helm install --name XXX .
helm delete --purge XXX
helm upgrade XXX .
helm rollback XXX 1
helm upgrade XXX . --set service.type=NodePort
```



