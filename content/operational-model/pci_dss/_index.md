TODO: Going through [PCI-DSS cloud computing information supplement](
https://www.pcisecuritystandards.org/pdfs/PCI_SSC_Cloud_Guidelines_v3.pdf?agreement=true&time=1601049724962) and write a document that reports point by point the requirements.
Similar to [CoalFire Doc](https://www.redhat.com/cms/managed-files/Red_Hat_OpenShift_Reference_Architecture_for_PCI_DSS_3.2.1_v1.0.pdf) for Openshift.

To be reported:

* Kubeconfig in registration controller PODs (is it crypted?). Evidence to add in the DOC.
* Encrypted traffic beween managed cluster and HUB cluster?
* Encrypted ETCD in managed Kubernetes solutions (AKS, EKS, IKS, GKE). Is the Encryption key supplied by customer?
* East-West traffic to be encrypted (IP-Sec or Service Mesh or some CNI ex Calico). Encyrption key supplied by customer? How this will impact `Submariner` or `Skupper`  or other Cross Cluster Services?