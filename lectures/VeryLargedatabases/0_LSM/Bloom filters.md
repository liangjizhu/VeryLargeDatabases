- Simple data structure to quickly check if a key may exist in a dataset
- Bitmap of **m** bits and **k** unique hash functions
- Either used on each block or the complete [[Sorted String Table]]
![[Pasted image 20251204162758.png]]

Internet:
A space-efficient, probabilistic data structure used to test if an element is a member of a set, with the warning that it can produce false positives but never false negatives.

How it works:
It uses a hash function to mark bits in a bit array, and when testing for membership, it says an element is "definitely not in the set" if any of its corresponding bits are not set. If all of the bits are set, the filter responds that the element "might be in the set", though it's possible this is a false positive. 