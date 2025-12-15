An indexing technique—commonly used in search engines—where documents are indexed by the terms (words or tokens) they contain. It enables fast keyword searches over large text collections.
- Term partitioned is also called [[Global Indexing]]
- Reads may become faster, but writes may become slower (they are not local). Updates may be done [[Asynchronous]] ([[Amazon Dynamo]]) 
![[Pasted image 20251211174214.png]]