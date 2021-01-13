
Goal of this document is to try to supply 

My cluster is going to be managed by ACM (join?):

   * Which information should I supply? You should supply _only_ the kubeadmin rights through `kubeconfig` file, with `kubeadmin` rights. See [PCI-DSS]({{< ref path="/operational-model/pci_dss/_index.md" >}})
   * How the registration will work?
   * Which resources ACM agent will need?
   * What  will be installed? See [APIs]({{< ref path="/content/apis/_index.md" >}}).
   * What if I want my cluster to unjoin the HUB cluster?

I want to host provision an HUB cluster:

   * What resources should I supply (VM size etc)?
   * Should the cluster be public available (disconnected mode)?


Policies:

   * Is there a way to have a timing windows for the policy? For example to grant 'software load config update only on Sunday'?

