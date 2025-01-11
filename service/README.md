| Service type | spec |  |
| --- | --- | --- |
| ClusterIP |  |  |
| NodePort |  |  |
| LoadBalancer |  |  |
| ExternalName |  |  |
|  |  |  |
| ClusterIP | clusterIP: None | [Headless Services](https://kubernetes.io/docs/concepts/services-networking/service/#headless-services) |
| Any Service | externalIPs: 1.2.3.4 | [External IPs](https://kubernetes.io/docs/concepts/services-networking/service/#external-ips) |

# Documentation
[Service type](https://kubernetes.io/docs/concepts/services-networking/service/#publishing-services-service-types)
