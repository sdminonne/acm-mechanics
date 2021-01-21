
Application Lifecycle exposes a UI for to handle subscriptions. [Official doc](https://access.redhat.com/documentation/en-us/red_hat_advanced_cluster_management_for_kubernetes/2.1/html/manage_applications/managing-applications)


Applications load/deployment in ACM follows a _subscription_ model. ACM adds `Placement Rule` to the usual subscription model.


<!-- prettier-ignore -->
<!-- spellchecker-disable -->
<!-- prettier-ignore -->
{{< mermaid class="text-center" >}}
sequenceDiagram
    participant Source
    participant Channel
    participant PlacementRule
    participant Subscription
    Subscription--xChannel: Watch
    activate Channel
    Subscription--xPlacementRule: Watch
    activate PlacementRule
    PlacementRule->>Subscription: Cluster(s) candidate
    deactivate PlacementRule
    Source->>Channel: Event (k8s Resource, Git commit, Storage change)
    Channel->>Subscription: New Resource
    deactivate Channel
{{< /mermaid >}}

<!-- spellchecker-enable -->



