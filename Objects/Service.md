A [service](https://kubernetes.io/docs/concepts/services-networking/service/) is a static ip address on the [[Kubernetes Virtual Network]] that can be attached to each pod.

Regardless of if a pod dies, a service bound to a particular pod will persist.

#### Types of Services
- NodePort: a service that exposes a Pod through a port on its [[Node]]
- ClusterIP: a service that creates a virtual IP to facilitate communication between different services within a [[Cluster]]
- LoadBalancer: creates/provisions a load balancer to a set of servers in a [[Cluster]]
- *ExternalName:* a service that maps to a specific internal ip. (Uncommon)


Services are generally best suited for communication between pods.
**For external connectivitiy, [[Ingress]] is often a more appropriate solution.**

