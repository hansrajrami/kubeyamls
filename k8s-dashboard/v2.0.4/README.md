### Get token to access dashboard 

```
kubectl get secret -n kubernetes-dashboard <token name of your service account> -o json | jq -r .data.token | base64 --decode
```
