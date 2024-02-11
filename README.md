# argocd-example-apps

My example argocd apps. These are intended to work with a K3s cluster runing Traefik for ingress

For example to import one with argocd into your K3s cluster

```
argocd app create nginxweb --repo https://github.com/mtcoffee/argocd-example-apps.git --path nginxweb --dest-server https://kubernetes.default.svc --dest-namespace default
argocd app sync nginxweb
```
