An abstract notion of time used in [[Distributed System]] to order events based on causality, rather than on physical clock time.
- Order of events
-  Focused on cause and effect
- Typically a counter increment for each event

- If we only need to order events, [[Physical Time]] is overkill
- Also, perfect synchronization of physical clocks is impossible !
- [[Local Time]] - Focus on event order
	- Two local events happened in the order observed by the process executing them
	- A message must be sent before it can be received
	- Example Cause - Effect