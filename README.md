# yarr

A Helm Chart for [yarr (Yet Another RSS Reader)](https://github.com/nkanaev/yarr) - a simple RSS reader.

## Building the Chart

```bash
helm package .
helm push yarr-*.tgz oci://ghcr.io/felixzmn/helm
```
