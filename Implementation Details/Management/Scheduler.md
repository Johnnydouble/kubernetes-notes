[Scheduler](https://kubernetes.io/docs/concepts/overview/components/#kube-scheduler) is a management service that determines what [[Node]] a new pod should be run on based on a number of factors.

The [[Scheduler]] inovokes [[Kublet]] in order to actually start the new [[Pod]] in a container.