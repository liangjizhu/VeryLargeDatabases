- Consider the following relational algebra expression in which the relations are neither replicated nor fragmented
			account ⋈ depositor ⋈ branch
	- Account is stored at site S_1
	- depositor ar S_2
	- Branch at S_3
- For a [[Queries]] issued at site S_i, the system needs to produce the result at site S_i
Possible strategies
- [[Ship Copies]] of all three relation to site S_i and choose a strategy for processing the entire locally at site S_i
- [[Ship Copies]] between sites
	- Ship a copy of account and compute temp_1 = account ⋈ depositor at S_2
	- Ship temp_1 to S_3, and compute temp_2 = temp_1 ⋈ branch at S_3
	- Ship the result temp_2 to S_i
- You must consider some important factors
	- Amount of data being shipped, cost of transmitting a data block between sites, relative processing speed at each site