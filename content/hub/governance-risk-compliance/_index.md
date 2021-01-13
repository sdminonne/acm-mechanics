## Policy propagation

WIP and an example of Sequence Diagram (TODO finalize it sequence diagram)

<!-- prettier-ignore -->
<!-- spellchecker-disable -->
<!-- prettier-ignore -->
{{< mermaid class="text-center" >}}
sequenceDiagram
    Hub->>Spoke1: Hi 'Spoke1' I've a 'policy' named 'Desire v1'
    loop AlreadyHave
        Spoke1->>Spoke1: Have I already 'Desire v1' policy?
    end
    Spoke1->>Hub: Send me the 'policy' 'Desire v1'
    opt Desirev1
        Hub->>Spoke1: Here is the policy
    end
    Spoke1->>Hub: Policy 'Desire v1' created
    
{{< /mermaid >}}

<!-- spellchecker-enable -->


