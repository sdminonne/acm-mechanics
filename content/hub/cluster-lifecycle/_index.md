

Cluster registration sequence diagram

<!-- prettier-ignore -->
<!-- spellchecker-disable -->
<!-- prettier-ignore -->
{{< mermaid class="text-center" >}}
sequenceDiagram
    participant Alice
    participant Hub
    participant Cluster1
    Cluster1--xHub: submit CSR
    activate Hub
    Alice->>Hub: CSR approval
    deactivate Hub
    Alice->>Hub: Cluster1 accepted
    Hub--xHub: Managing Cluster1
    Alice->>Hub: submit ManifestWork

{{< /mermaid >}}

<!-- spellchecker-enable -->


TODO: adds explanation about [Hive Operator](https://www.openshift.com/blog/openshift-hive-cluster-as-a-service). 

<!-- https://github.com/open-cluster-management/cluster-lifecycle-e2e/blob/main/e2e-test/open_cluster_management_e2e_suite_test.go -->