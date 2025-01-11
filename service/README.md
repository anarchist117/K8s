| Service type | spec |
| --- | --- |
| [ClusterIP](https://kubernetes.io/docs/concepts/services-networking/service/#type-clusterip) |  |
| [NodePort](https://kubernetes.io/docs/concepts/services-networking/service/#type-nodeport) | type: NodePort |
| [LoadBalancer](https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer) | type: LoadBalancer |
| [ExternalName](https://kubernetes.io/docs/concepts/services-networking/service/#externalname) | type: ExternalName |
|  |  |
| **Service Extended** | **spec** |
| [Headless Services](https://kubernetes.io/docs/concepts/services-networking/service/#headless-services) | clusterIP:   None |
| [External IPs](https://kubernetes.io/docs/concepts/services-networking/service/#external-ips) | externalIPs: 1.2.3.4 |

# Documentation
[Service type](https://kubernetes.io/docs/concepts/services-networking/service/#publishing-services-service-types)
