# Setup

```
helm upgrade --install ingress-nginx ingress-nginx \
  --repo https://kubernetes.github.io/ingress-nginx \
  --namespace ingress-nginx --create-namespace \
  --values ingress-nginx-values.yaml
```

Manually (through the upcloud web UI) create a dynamic certificate bundle for the target domain (e.g. dev.phnx.im) on the frontend and activate TLS and HTTP2 in the backend. Note that after manual configuration through the UI, the loadbalancer can't be configured anymore through Helm.
