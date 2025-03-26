# helm-yarr

A Helm Chart for [yarr (Yet Another RSS Reader)](https://github.com/nkanaev/yarr) - a simple RSS reader.

## Building the Chart

```bash
helm package .
helm registry login ghcr.io -u felixZmn

export CHART_VERSION=$(grep -m 1 'version:' ./Chart.yaml | tail -n1 | awk '{ print $2 }')
helm push yarr-*.tgz oci://ghcr.io/felixzmn/helm
```
