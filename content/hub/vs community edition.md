Goal of this section is to present differences between _community edition_ and `RHACM`. What here we call _community edition_ is what can be found at [https://open-cluster-management.io](https://open-cluster-management.io/)



## Deployments

| Namespace               | RHACM | _community_ | Comments |
|:-----                   |:----------------------------- |:-------- |:---- |
| hive                                 | hive-controllers | - |  Currently no hive namespace in _community edition_ |
| hive                                 | hiveadmission | - |  Currently no hive namespace in _community edition_ |
| olm                                  | - | catalog-operator |  - |
| olm                                  | - | olm-operator  |  - |
| olm                                  | - | packageserver  | - | - |
| openshift-operator-lifecycle-manager | catalog-operator |  - | - |
| openshift-operator-lifecycle-manager | olm-operator  |  - | - |
| openshift-operator-lifecycle-manager | packageserver  |  - | - |
| open-cluster-management     | application-chart-3729c-applicationui | - | - |
| open-cluster-management     | cert-manager-ac739 | - |  To be removed in 2.3 |
| open-cluster-management     | cert-manager-webhook | - | To be removed in 2.3 |
| open-cluster-management     | cert-manager-webhook-28982-cainjector  | - |  To be removed in 2.3 |
| open-cluster-management     | cluster-manager | cluster-manager |  - |
| open-cluster-management     | configmap-watcher-9916f  | - | it watches `cert-manager-webhook` configmap. It restarts the webhook on configmap updates. It will disappear in 2.3 |
| open-cluster-management     | console-chart-36b82-consoleapi | - |
| open-cluster-management     | console-chart-36b82-consoleui | - |
| open-cluster-management     | console-header | - |  - |
| open-cluster-management     | grc-b63ce-grcui | - |  - |
| open-cluster-management     | grc-b63ce-grcuiapi | - |  - |
| open-cluster-management     | grc-b63ce-policy-propagator | - |  - |
| open-cluster-management     | hive-operator | - |  - |
| open-cluster-management     | klusterlet-addon-controller | - |  - |
| open-cluster-management     | kui-web-terminal | - |  - |
| open-cluster-management     | managedcluster-import-controller | - |  - |
| open-cluster-management     | management-ingress-e95f4 | - |  - |
| open-cluster-management     | multicluster-observability-operator | - |  - |
| open-cluster-management     | multicluster-operators-application | - |  - |
| open-cluster-management     | multicluster-operators-hub-subscription | - |  - |
| open-cluster-management     | multicluster-operators-standalone-subscription | - |  - |
| open-cluster-management     | multiclusterhub-operator | - |  - |
| open-cluster-management     | multiclusterhub-repo | - |  - |
| open-cluster-management     | ocm-controller | - |  - |
| open-cluster-management     | ocm-proxyserver | - |  - |
| open-cluster-management     | ocm-webhook| - |  - |
| open-cluster-management     | search-operator | - |  - |
| open-cluster-management     | search-prod-f8911-redisgraph | - |  - |
| open-cluster-management     | search-prod-f8911-search-aggregator | - |  - |
| open-cluster-management     | search-prod-f8911-search-api | - |  - |
| open-cluster-management     | search-prod-f8911-search-collector | - |  - |
| open-cluster-management     | topology-62a7d-topology | - |  - |
| open-cluster-management     | topology-62a7d-topologyapi | - |  - |
| open-cluster-management-hub | cluster-manager-registration-controller | cluster-manager-registration-controller |  - |
| open-cluster-management-hub | cluster-manager-registration-webhook | cluster-manager-registration-webhook |  - |
| open-cluster-management-hub | cluster-manager-work-webhook  | cluster-manager-work-webhook |  - |
| open-cluster-management-agent       | - | - |  - |
| open-cluster-management-agent-addon | - | - |  - |

## Certs

| Namespace               | RHACM | _community_ | Comments |
|:-----                   |:----------------------------- |:-------- |:---- |
| open-cluster-management | application-chart-3729c-applicationui-ca-cert | - |  No cert manager in _community edition_ (Future?) |
| open-cluster-management |console-chart-36b82-ca-cert | - |  No cert manager in _community edition_ (Future?) |
| open-cluster-management |grc-b63ce-ca-cert | - |  No cert manager in _community edition_ (Future?) |
| open-cluster-management |kui-proxy | - |  No cert manager in _community edition_ (Future?) |
| open-cluster-management |management-ingress-e95f4-cert | - |  No cert manager in _community edition_ (Future?) |
| open-cluster-management |multicloud-ca-cert | - |  No cert manager in _community edition_ (Future?) |
| open-cluster-management |search-aggregator-ca-cert | - |  No cert manager in _community edition_ (Future?) |
| open-cluster-management |search-prod-f8911-redis-ca-cert | - |  No cert manager in _community edition_ (Future?) |
| open-cluster-management |search-prod-f8911-search-ca-cert | - |  No cert manager in _community edition_ (Future?) |
| open-cluster-management |topology-62a7d-ca-cert | - |  No cert manager in _community edition_ (Future?) |
