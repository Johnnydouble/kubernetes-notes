[Ingress](https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.26/#ingress-v1-networking-k8s-io) exposes HTTP and HTTPS routes from outside the cluster to [[Service|Services]] within the cluster. Traffic routing is controlled by rules defined on the Ingress resource.

Ingress is often used to terminate SSL

#### Ingress Components
-  ### **Ingress Controller:**
	- A proxy/load balancer that manages ingress based on provided rules
	- Available Controllers:
		- Official (as of 2022):
			- [NGINX](https://git.k8s.io/ingress-nginx/README.md#readme)
			- [GCE](https://git.k8s.io/ingress-gce/README.md#readme)
			- [AWS](https://github.com/kubernetes-sigs/aws-load-balancer-controller#readme)
		- Unofficial:
			- [Istio Ingress](https://istio.io/latest/docs/tasks/traffic-management/ingress/kubernetes-ingress/)
			- all others (see [Additional Controllers](https://kubernetes.io/docs/concepts/services-networking/ingress-controllers/#additional-controllers))
- **Ingress Resources:**
	- Rules that let you configure how incomming traffic is routed
	- Each rule contains:
		- A host (optional)
			- EX: `foo.bar.com`
		- A list of paths:
			- Each list has an associated backend with ONE of the following:
				- A Service (with  `service.name`, `service.port.name` or `service.port.number`)
				- A Resource
			- EX: `/testpath`
			- NOTE: hoest and path must match incomming content before the traffic is directed onto the given backend
	- 