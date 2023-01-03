The [Cloud Controller Manager](https://kubernetes.io/docs/concepts/overview/components/#cloud-controller-manager) is a component that allows for better integration between a cluster and a cloud provider's api.

Each implementation is cloud provider specific because it must couple to said provider's API.

The [[Cloud Controller Manager]] is useful for configuring routes between nodes, integrating with cloud infra components including managed load balancers, packet filters, integrating with authorization and more.
