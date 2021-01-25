## Managed Cluster resources

| Namespace                           | RHACM | _community_            | Comments |
|--------                             |:----- |:---------------------  |:-------- |
| olm                                 | -     | catalog-operator       | -                         |
| open-cluster-management             | -                              | klusterlet                |  RHACM `klusterlet` runs in `open-cluster-management-agent`  workspace |
| open-cluster-management             | -                              | klusterlet-registry-server    |  - |
| open-cluster-management-agent       | klusterlet                     | -                             |  _community_ `klusterlet` runs in  `open-cluster-management` workspace |
| open-cluster-management-agent       | klusterlet-registration-agent  | klusterlet-registration-agent |  - |
| open-cluster-management-agent       | klusterlet-work-agent          | klusterlet-work-agent         |  - |
| open-cluster-management-agent-addon | -                              | -                             |  - | 