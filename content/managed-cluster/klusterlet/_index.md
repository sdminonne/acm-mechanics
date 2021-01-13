
```math
klusterlet : ACM = kubelet : kubernetes`
```

`klusterlet` as the name suggests, is to `ACM` as `kubelet` is to `kubernetes`, more prosaically, is the `ACM` _agent_ on the managed cluster.

## Klusterlet registration flow

<!-- prettier-ignore -->
<!-- spellchecker-disable -->
<!-- prettier-ignore -->
{{< mermaid class="text-center" >}}
sequenceDiagram
    Hub->>Spoke1: foo bar
    
    Spoke1->>Spoke1: ratplan
    Spoke1->>Hub: Send me the 'policy' 'Desire v1'
    opt Desirev1
        Hub->>Spoke1: Here is the policy
    end
    Spoke1->>Hub: Policy 'Desire v1' created
    
{{< /mermaid >}}

<!-- spellchecker-enable -->