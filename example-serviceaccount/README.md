```bash
kubectl apply -f admin-serviceaccount.yml
kubectl create token admin-sa
kubectl get pods --token="<TOKEN>" --server="https://192.168.49.2:8443" --insecure-skip-tls-verify
```
