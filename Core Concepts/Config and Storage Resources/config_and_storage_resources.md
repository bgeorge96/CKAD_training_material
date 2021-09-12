# Config and Storage Resources

## ConfigMap  

A ConfigMap holds configuration data for pods to consume ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/config-map-v1/)).

## Secret  

A Secret holds secret data of a certain type ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/secret-v1/)). [Additional Resource](https://www.tutorialspoint.com/kubernetes/kubernetes_secrets.htm)

## Volume  

A Volume represents a named volume in a pod that may be accessed by any container in the pod ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/volume/)). [Additional Resource](https://www.tutorialspoint.com/kubernetes/kubernetes_volumes.htm)

## PersistentVolumeClaim  

A PersistentVolumeClaim is a user's request for and claim to a persistent volume ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-claim-v1/)). 

## PersistentVolume  

A PersistentVolume (PV) is a storage resource provisioned by an administrator ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-v1/)).

## StorageClass  

A StorageClass describes the parameters for a class of storage for which PersistentVolumes can be dynamically provisioned ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/storage-class-v1/))

## Volume Attachment  

A VolumeAttachment captures the intent to attach or detach the specified volume to/from the specified node ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/volume-attachment-v1/)).

## CSIDriver  

A CSIDriver captures information about a Container Storage Interface (CSI) volume driver deployed on the cluster ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/csi-driver-v1/)).

## CSINode  

A CSINode holds information about all CSI drivers installed on a node ([Doc Link](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/csi-node-v1/)).
