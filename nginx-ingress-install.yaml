# Nginx Ingress Controller
## **Install Helm**

On each K3s node where you want to run a Prometheus instance (or node exporter), install Helm:

```bash
curl https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3 | bash
```

Verify Helm installation:

```bash
helm version
```
### **Install NGINX Ingress Controller**

Recommended way is using Helm:

```bash
helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx
helm repo update

kubectl create namespace ingress-nginx

helm install ingress-nginx ingress-nginx/ingress-nginx \
  --namespace ingress-nginx
```

This will deploy the NGINX ingress controller in your cluster.
