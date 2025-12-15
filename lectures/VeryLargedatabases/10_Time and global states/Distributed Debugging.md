- How did variables change at runtime ?
	- Example: Has |x_1 - x_2| ever been > 50 ?
- Variables can be located at different processes / nodes
- Prolem: Global consistent view of variable values
![[Cuts]]

- After the fact: Was a condition true during execution ?
- All participants send information about state changes to an external observer
- Global state predicate þ
	- Possibly þ
		- At least one [[Consistent]] run passes through a global [[Consistent]] state where þ = true
	- Definitely þ
		- All [[Consistent]] runs pass through a global [[Consistent]] state where þ = true
