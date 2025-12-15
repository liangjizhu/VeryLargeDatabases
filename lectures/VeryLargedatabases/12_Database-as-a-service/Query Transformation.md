- Translating algebraic [[Queries]] on fragments
	- It must be possible to construct relation r from its fragments
	- Replace relation r by the expression to construct r from its fragments
- Consider the [[Horizontal Partitioning]] of account
		account_1 = σ_(brach = "Hillside")(account)
		account_2 = σ_(brach = "Valleyview")(account)
- Consider the following query
		σ_(brach = "Hillside")(account) => 
		σ_(brach = "Hillside")(account_1 U account_2) =>
		σ_(brach = "Hillside")(account_1) U σ_(brach = "Hillside")(account_2) =>
		σ_(brach = "Hillside")(account_1)
![[Simple Join]]