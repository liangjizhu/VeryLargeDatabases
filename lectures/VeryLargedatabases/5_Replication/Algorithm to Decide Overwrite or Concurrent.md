- Server maintains version number for every key, increments version number at writes
- At read, the version number is returned. A client read before write
- When writing, it must include the version number of the read. And merge in all vales received in the previous read
- When the server receives a write with a (read) version number, it can overwrite all values with that read version number and lower.
	But it must keep all values with a higher version number (They are "[[Concurrency]]")
	