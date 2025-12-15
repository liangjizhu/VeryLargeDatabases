The most severe type of failure in a [[Distributed System]], where a node behaves arbitrarily or maliciously. Instead of simply crashing or becoming slow, a faulty node may:
- Lie
- Send conflicting information to different nodes
- Pretend to be different nodes
- Omit or alter messages
- Act correctly sometimes and incorrectly other times

We assume that nodes are unreliable, but honest: They may be slow or never respond, and their state may be outdated. But they never "lie"
- If a node tells a "lie", everything becomes harder: [[Byzantine Faults]]
- Aerospace applications need to tolerate [[Byzantine Faults]] (cosmic radiation)
- [[Bitcoin]] / [[Blockchains]] need to tolerate [[Byzantine Faults]] (fraud)
- A bug in the software could be regarded as a [[Byzantine Faults]], but if you deploy the same software to all nodes, then a [[Byzantine Faults]]-tolerant algorithm cannot save you