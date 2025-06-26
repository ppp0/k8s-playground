# Kubernetes/Helm Playground

Some sample Helm charts to deploy a Nginx server and an Ingress to play around with various aspects of Helm

## Prerequisites
- Docker, Podman or other cri-o platform supported by Kind
- [kind](https://kind.sigs.k8s.io/)
- [kubectl](https://kubernetes.io/docs/reference/kubectl/) or [oc](https://docs.redhat.com/en/documentation/openshift_container_platform/4.10/html/cli_tools/openshift-cli-oc)
- [Helm](https://helm.sh/)

Optional:
- [Helm diff Plugin](https://github.com/databus23/helm-diff)

## Installation
- Clone this repository, cd into it
- Start Kind
```shell
kind create cluster --config=kind/config.yaml
```
- Deploy application
```shell
helm install nginx-with-ingress nginx-with-ingress/
```
- Browse to http://localhost

