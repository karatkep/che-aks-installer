# che-aks-installer
## Define env variables:
```
export TENANT_ID=
export AUTH_CLIENT_ID=
export AUTH_CLIENT_SECRET=
export CHE_DOMAIN=
```
## Command to install

```
chectl server:deploy --installer operator -p k8s --skip-oidc-provider-check \
    --che-operator-image=docker.io/karatkep/che-operator:beta \
    --domain=${CHE_DOMAIN} \
    --che-operator-cr-patch-yaml=che-cluster.yml
```
