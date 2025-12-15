- Every process has a logical clock (counter) L_i
- Before every event: L_i = L_i + 1
- Attach clock value to every message, t = L_i
- When receiving, L_j = max(L_j, t) + 1
![[Pasted image 20251213044905.png]]
- If e -> e' then L(e) < L(e')
- But the reverse is not true !
	- L(e) < L(b) without e -> b
	- But L(e') > L(e) -> (not e' -> e)
![[Pasted image 20251213045211.png]]

Try yourselves !
![[Pasted image 20251213045315.png]]
- What are the logical clock values ?
- Is d -> g ?
- Is a -> g ?