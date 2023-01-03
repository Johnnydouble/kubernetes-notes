A Job is a [[Workload Resource]] that represents one-off tasks.

A Job creates one or more Pods and will continue to retry execution of the Pods until a specified number of them successfully terminate. 

Completions are tracked and when the specified number of them are sucessfully reached, the job is complete.

Deleting a job will clean up its consitutent pods, and suspending will delete its active pods until the job is resumed.