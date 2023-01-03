A consistent, highly-available, (often distributed) key value store that holds a [[Cluster]]'s state.

Every change to the [[Cluster]] is reflected in [[etcd]] (pod creation, deletion, jobs, etc).

**Note: application data is not stored in [[etcd]]**

