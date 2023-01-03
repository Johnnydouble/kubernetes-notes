An abstraction over a container (or occasionally containers); The smallest unit of K8S.

Allows you to interact with containerized applications without having to worry about the  specifics of the containerization platform.

## Each Pod Has:
- **1 .. n** containers (best practice is to use 1 or one main container and helpers)
- **Exactly 1** IP address within the [[Kubernetes Virtual Network]]
- Pods are ephemeral and can die
	- When a pod is recreated, a new IP will be assigned
	- [[Service|Services]] can be created to obviate the need to manage reassignment of ip references when a pod dies, similar to a static ip