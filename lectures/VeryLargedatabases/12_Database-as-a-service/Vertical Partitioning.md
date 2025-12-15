The [[Schemas]] for the relation r is split into several smaller [[Schemas]]
- All [[Schemas]] must contain a common candidate key (or superkey) to ensure the lossless join property
- A special attribute, the tuple-id attribute, may be added to each [[Schemas]] to serve as a candidate key
![[Pasted image 20251214214414.png]]

Advantages:
- Allows tuples to be split so that each part of the tuple is stored where it is most frequently accessed
- Tuple-id attribute allows efficient joining of vertical fragments
- Allows [[Parallel Execution]] on a relation