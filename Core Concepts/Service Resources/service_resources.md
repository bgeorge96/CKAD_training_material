# Workload Resources  

## Service  

A Service is a named abstraction of software service (for example, mysql) consisting of local port (for example 3306) that the proxy listens on, and the selector that determines which pods will answer requests sent through the proxy ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/service-resources/service-v1/)). [Addition Resource](https://www.tutorialspoint.com/kubernetes/kubernetes_service.htm)  

## Endpoints  

Endpoints is a collection of endpoints that implement the actual service. Example: Name: "mysvc", Subsets: [ { Addresses: [{"ip": "10.10.1.1"}, {"ip": "10.10.2.2"}], Ports: [{"name": "a", "port": 8675}, {"name": "b", "port": 309}] }, { Addresses: [{"ip": "10.10.3.3"}], Ports: [{"name": "a", "port": 93}, {"name": "b", "port": 76}] }, ] ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/service-resources/endpoints-v1/)). This article has a really good example of what endpoints are used for ([Article](https://theithollow.com/2019/02/04/kubernetes-endpoints/)). TLDR: They allow you to configure external (outside of k8s cluster) api calls in a service familiar k8s format.

## Ingress  

Ingress is a collection of rules that allow inbound connections to reach the endpoints defined by a backend. An Ingress can be configured to give services externally-reachable urls, load balance traffic, terminate SSL, offer name based virtual hosting etc ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/service-resources/ingress-v1/)). 
