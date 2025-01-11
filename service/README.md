| Service type | spec | Description |
| :--- | :--- | :--- |
| [ClusterIP](https://kubernetes.io/docs/concepts/services-networking/service/#type-clusterip) |  |  |
| [NodePort](https://kubernetes.io/docs/concepts/services-networking/service/#type-nodeport) | type: NodePort |  |
| [LoadBalancer](https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer) | type: LoadBalancer |  |
| [ExternalName](https://kubernetes.io/docs/concepts/services-networking/service/#externalname) | type: ExternalName |  |
|  |  |
| **Service extended** | **spec** | **Description** |
| [Headless Services](https://kubernetes.io/docs/concepts/services-networking/service/#headless-services) | clusterIP: None | A headless Service allows a client to connect to whichever Pod it prefers, directly |
| [External IPs](https://kubernetes.io/docs/concepts/services-networking/service/#external-ips) | externalIPs: 1.2.3.4 | Kubernetes Services can be exposed on those externalIPs |
