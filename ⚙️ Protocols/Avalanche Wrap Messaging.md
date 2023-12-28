---
aliases:
  - AWM
---
[[Avalanche Wrap Messaging|AWM]] enables native cross-Subnet communication and allows Virtual Machine[ˆ1]  developers to implement arbitrary communication protocols between any two Subnets.[ˆ2]
## Cross-Subnet Communication

![[Pasted image 20231215085125.png]]

[[Avalanche Wrap Messaging|AWM]] can send any arbitrary array of bytes to other subnets and it uses the BLS Signature Scheme[ˆ3] where each validator on the Avalanche Network holds a key pair.

Validators of one subnet can individually sign a message and those signatures are aggregated into a short multi-signature that can be verified quickly (BLS properties).


[ˆ1]: https://docs.avax.network/learn/avalanche/subnets-overview#virtual-machines
[ˆ2]: https://docs.avax.network/learn/avalanche/awm
[ˆ3]: https://crypto.stanford.edu/~dabo/pubs/papers/BLSmultisig.html