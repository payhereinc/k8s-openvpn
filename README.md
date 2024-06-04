# K8s-OpenVPN

Repository contains information on how to build, install and configure OpenVPN for kubernetes cluster.

Inspired by

- <https://github.com/kylemanna/docker-openvpn>
- <https://github.com/helm/charts/tree/master/stable/openvpn>
- <https://tech.kutumb.app/simplifying-kubernetes-service-access-with-openvpn-a-complete-production-guide>



## Apply Helm Chart
```shell
cd deploy/openvpn

$ helm template openvpn ./ -n security -f values.yaml > test.yaml

$ helm upgrade openvpn ./ -n security -f values.yaml
```
