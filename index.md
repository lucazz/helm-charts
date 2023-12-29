# Lucas' Helm Charts

<!--toc:start-->
- [Lucas' Helm Charts](#lucas-helm-charts)
  - [Add Helm repository](#add-helm-repository)
    - [Dependencies](#dependencies)
<!--toc:end-->

[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/lucazz/helm-charts?style=for-the-badge)](https://github.com/lucazz/helm-charts/releases/latest)

This repository hosts Lucas's [Helm](https://helm.sh) charts.
Chart documentation is automatically generated using [helm-docs](https://github.com/norwoodj/helm-docs)

## Add Helm repository

```bash
helm repo add lucazz https://www.saboya.pro/helm-charts/
helm repo update
```

### Dependencies
Most of these charts are built to host tolling I use in my home setup, which relies on [Canonical's MicroK8s](https://microk8s.io/). These are the plugins I have installed in my cluster:

- [CoreDNS](https://microk8s.io/docs/addon-dns)
- [HostPath-Storage](https://microk8s.io/docs/addon-hostpath-storage) 
- [Ingress](https://microk8s.io/docs/addon-ingress)

You can install them by issuing this following commands:
```bash
microk8s enable dns
microk8s enable hostpath-storage
microk8s enable ingress
```
