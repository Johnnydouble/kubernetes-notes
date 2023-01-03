[Kublet](https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet/#synopsis) is an intermediary between the Kubernetes control plane and the [[Node|Nodes]] running the workload.

One instance runs per node (//todo:factcheck)

### Kublet Responsibilties:
- Running pods desired by the control plane
- Informing the cluster when its node has joined the cluster
- Reporting node and pod status

Kublet itself works in terms of a Podspec (a JSON/YAML description of a pod) and attempts to maintain consistancy between a given set of podspecs and cluster state