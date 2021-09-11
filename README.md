# CKAD Training Material

This is going to be a compilation of the material that is suggested from the CKAD_Curriculum_V1_21.pdf in this repo. I am planning on taking this certification here towards the end on 2021 and wanted to make a place to hold some of the objects that could be helpful for others. 

## Learning by Doing

The goal of this repo is to provide some hands on experiences where possible to get some learning by doing different K8s things. Where applicable I intent to make folders of problems to help people work through. 

If you feel like you need to get up to speed on K8s and some of the basics this Pluralsight video course might be a good place to start: https://app.pluralsight.com/paths/certificate/certified-kubernetes-application-developer-ckad

## Objectives to be Covered

This will be the same objectives as in the pdf mentioned above. I plan to add resources that I find helpful along the way to help with getting up to speed. 

### Core Concepts

- Understand Kubernetes API primitives
    - [K8s API Resources Docs](https://kubernetes.io/docs/reference/kubernetes-api/)
- Create and configure basic Pod
    - [Pods Docs](https://kubernetes.io/docs/concepts/workloads/pods/)
    - [Different guides to helping setup pods](https://kubernetes.io/docs/tasks/configure-pod-container/)

### Configuration

- Understand ConfigMaps
    - [ConfigMap Docs](https://kubernetes.io/docs/concepts/configuration/configmap/)
    - [Configuring pod to use ConfigMap](https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/)
- Understand SecurityContexts
    - [PodSecurityContext Docs](https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.22/#podsecuritycontext-v1-core)
    - [SecurityContexts for a pod or container](https://kubernetes.io/docs/tasks/configure-pod-container/security-context/)
- Define an application's resource requirements
    - [Assigning Memory for Pod](https://kubernetes.io/docs/tasks/configure-pod-container/assign-memory-resource/)
    - [Assigning CPU for a Pod](https://kubernetes.io/docs/tasks/configure-pod-container/assign-cpu-resource/)
- Create & consume Secrets
    - [Secrets Docs](https://kubernetes.io/docs/concepts/configuration/secret/)
    - [Creating and using Secrets](https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/)
- Understand ServiceAccounts
    - [Setting up ServiceAccounts for a pod](https://kubernetes.io/docs/tasks/configure-pod-container/configure-service-account/)
    - [Managing Service Accounts (might be out of scope TBD)](https://kubernetes.io/docs/reference/access-authn-authz/service-accounts-admin/)

### Multi-Container Pods

- Understand Multi-Container Pod design patterns (e .g. ambassador, adapter, sidecar)
    - [Multicontainer course in PluralSight](https://app.pluralsight.com/library/courses/kubernetes-developers-integrating-volumes-using-multi-container-pods)
    - [Article about different container design patterns](https://kubernetes.io/blog/2015/06/the-distributed-system-toolkit-patterns/)

### Observability

- Understand LivenessProbes and ReadinessProbes
    - [Setting up readiness and liveness on a pod](https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/)
- Understand container logging
- Understand how to monitor applications in Kubernetes
- Understand debugging in Kubernetes
    - [Link for Tasks to help with three prior points](https://kubernetes.io/docs/tasks/debug-application-cluster/)

### Pod Design

- Understand Deployments and how to perform rolling updates
    - [Deployment Rolling Update](https://kubernetes.io/docs/tutorials/kubernetes-basics/update/update-intro/)
- Understand Deployments and how to perform rollbacks
    - [Performing a Roll Back](https://kubernetes.io/docs/tutorials/kubernetes-basics/update/update-intro/)
- Understand Jobs and CronJobs
    - [Jobs Docs](https://kubernetes.io/docs/concepts/workloads/controllers/job/)
    - [CronJobs Docs](https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/)
- Understand how to use Labels, Selectors, and Annotations
    - [Labels and Selectors Docs](https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/)
    - [Annotations Docs](https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations/)

### Services and Networking

- Understand Services
    - [Services Docs](https://kubernetes.io/docs/concepts/services-networking/service/)
- Demonstrate basic understanding of NetworkPolicies
    - [Network Policies Docs](https://kubernetes.io/docs/concepts/services-networking/network-policies/)

### State Persistence

- Understand PersistentVolumeClaims for storage
    - [PersistentVolume Docs](https://kubernetes.io/docs/concepts/storage/persistent-volumes/)
    - [Running a Stateful application](https://kubernetes.io/docs/tasks/run-application/run-single-instance-stateful-application/)

## Links

- https://www.cncf.io/certification/ckad/
- https://kubernetes.io/docs/home/