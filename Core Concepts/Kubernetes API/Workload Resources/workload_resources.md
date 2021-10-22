# Workload Resources  

## Pod  

A Pod is a collection of containers that can run on a host. This resource is created by clients and scheduled onto hosts ([Doc Link](https://kubernetes.io/docs/concepts/workloads/pods/)). [Additional Resource](https://www.tutorialspoint.com/kubernetes/kubernetes_pod.htm)  

## PodTemplate  

A PodTemplate describes a template for creating copies of a predefined pod ([Doc Link](https://kubernetes.io/docs/concepts/workloads/pods/#pod-templates)). A PodTemplate is used in a Deployment to for it to know what type of pod to create ([Deployment Doc](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/)).  

## ReplicationController  

A ReplicationController represents the configuration of a replication controller ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/replication-controller-v1/)). This is the work horse of k8s that helps control and monitor the lifecycle of Pods ([ReplicationController TutorialsPoint](https://www.tutorialspoint.com/kubernetes/kubernetes_replication_controller.htm)).  

## ReplicaSet  

A ReplicaSet ensures that a specified number of pod replicas are running at any given time ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/replica-set-v1/)). [More About](https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/). This is similar to above, but the major difference is in the way that is is able to evaluate and find matching selectors. [Described here.](https://www.tutorialspoint.com/kubernetes/kubernetes_replica_sets.htm)  

## Deployment  

A Deployment enables declarative updates for Pods and ReplicaSets ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/deployment-v1/)). [More About](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/). [Additional Resource](https://www.tutorialspoint.com/kubernetes/kubernetes_deployments.htm)  

## StatefulSet  

StatefulSet represents a set of pods with consistent identities. Identities are defined as:  
- Network: A single stable DNS and hostname.  
- Storage: As many VolumeClaims as requested. The StatefulSet guarantees that a given network identity will always map to the same storage identity  
- ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/stateful-set-v1/))  
- [More About](https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/)

## DaemonSet

A DaemonSet represents the configuration of a daemon set ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/daemon-set-v1/s)). [More About](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/). DaemonSets are used to deploy a pod to every node in a cluster.  

## Job  

A Job represents the configuration of a single job ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/job-v1/)). [More Info](https://kubernetes.io/docs/concepts/workloads/controllers/job/). [Additional Resource](https://www.tutorialspoint.com/kubernetes/kubernetes_jobs.htm). A job is considered complete when a number of jobs completes successfully from the definition.  

## CronJob  

A CronJob represents the configuration of a single cron job ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/cron-job-v1/)). [More Info](https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/). This seems to be an extension of the scheduling capabilities of a Job, but with the granularity of cron syntax.  

## Additional Resources

### HorizontalPodAutoscaler

A HorizontalPodAutoscaler is a configuration of how to scale pods ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/horizontal-pod-autoscaler-v1/)).  

### PriorityClass  

A PriorityClass defines mapping from a priority class name to the priority integer value. The value can be any valid integer ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/priority-class-v1/)).