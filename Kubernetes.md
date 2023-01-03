Kubernetes aka k8s is a container orchestration platform that allows you to abstract the underlying  hardware, manage applications less closely, and maintain a **consistent, declarative state for application operations**. 

### Makeup
- A Kubernetes [[Cluster]] is a group of managed [Node](obsidian://open?vault=Kubernetes&file=Kubernetes%20Concepts%2FPhysical%20Abstractions%2FNode) having **1 to n [[Master Node|Master Nodes]]** and **0 to n**  [[Worker Node|Worker Nodes]]. 
	- Master Nodes handle management tasks, and can themselves also perform the role of Worker Nodes.
	- [etcd](obsidian://open?vault=Kubernetes&file=Kubernetes%20Implementation%20Details%2FManagement%2Fetcd), a distributed key-value store allows the management of clusters to be highly reliable and tolerant of losing one or multiple [[Master Node|Master Nodes]].

### Key Features:
- [[Horizontal Scaling]]
- [[Self-healing]]
- [[Load Balancing]] and [[Service|Service Discovery]]
- [[Secret]] & [[ConfigMap|Configuration Management]]
- [[Deployment|Automated rollouts and rollbacks]] (also see [[Workload]])
- [[Volumes|Storage Orchestration]]
- [[Job||Batch Execution]]
- [[Binpacking|Automatic Binpacking]]




### Trivia:
- In the abbreviation `k8s`, the 8 represents the 8 letters between the k and the s:  `k[ubernete]s`
- The name comes from the Greek word κυβερνήτης for *helmsman* or *ship pilot*