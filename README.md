# j1cken.github.io
j1cken's GitHub [Blog](https://j1cken.github.io)

## Helm Chart Repo
j1cken's Helm [Charts](https://j1cken.github.io/helm-charts)

Add to OpenShift with:
```
cat <<EOF | oc create -f -
apiVersion: helm.openshift.io/v1beta1
kind: HelmChartRepository
metadata:
  name: j1cken-repo
spec:
  connectionConfig:
    url: https://j1cken.github.io/helm-charts
EOF
```
