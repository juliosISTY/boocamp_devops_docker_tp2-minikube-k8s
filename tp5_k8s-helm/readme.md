## Install Helm v3
```sh
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh
```
You can check it with **helm version**

## Add Bitnami repository and install Wordpress
```sh
helm repo add bitnami https://charts.bitnami.com/bitnami
helm install wordpress bitnami/wordpress -f values.yml
```
And then verify if services and pods are created and running in your k8s cluster
Finaly, test in your browser

To uninstall wordpress run:

>helm delete wordpress
 
