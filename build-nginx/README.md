
# Crear POD desde el .yaml

```bash
kubectl create -f nginx.yaml
```
---

# Exponer el puerto
```bash
kubectl expose pod nginx --name=nginx-node-port-svc --port=80 --type=NodePort
```
> En este caso, ya deberia exponer el puerto y si no hacer un port-forwarding

```bash
kubectl port-forward nginx 8080:80
```
