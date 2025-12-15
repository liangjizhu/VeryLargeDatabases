- An operation B depends on another operation A, when the user/transaction has read A's value
- A [[Happens-Before]] B, or B is causally dependent on A
- An operation A [[Happens-Before]] another operation B if B knows about A, or depends on A, or builds upon A in some way.
- Two operations are [[Concurrency]] if neither [[Happens-Before]] the other
- Exact time doesn't matter: We simply call two operations [[Concurrency]] if they are both unaware of each other
![[Capturing the Happens-Before Relationship]]