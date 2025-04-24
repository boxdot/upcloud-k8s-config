# Setup

Upgrading the managed Load Balancer and ingress controller:

```
helm upgrade --install ingress-nginx ingress-nginx \
  --repo https://kubernetes.github.io/ingress-nginx \
  --namespace ingress-nginx --create-namespace \
  --values ingress-nginx-values.yaml
```
