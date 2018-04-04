# ucp

### Accès au Dashboard

Génère le token d'accès

```bash
kubectl -n kube-system describe secret $(kubectl -n kube-system get secret | grep admin-user | awk '{print $1}')
```