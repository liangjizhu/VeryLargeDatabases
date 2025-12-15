- A request arrives from the client in the [[Database Layer]] and is received by the [[Off-Chain Verifier]]
- The [[Off-Chain Verifier]] then forwards the request to an internal queue
- The [[Transaction Manager]] polls the request and processes it
- A put / get - request is created and is forwarded to the [[Shard Manager]]
- The [[Backend Connector]] accesses the [[Blockchains]] that stores the data
![[Pasted image 20251215020606.png]]