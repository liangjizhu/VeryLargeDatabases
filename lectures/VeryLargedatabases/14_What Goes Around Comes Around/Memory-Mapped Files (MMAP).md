Use the operating system’s virtual memory mechanism to map a file on disk directly into a process’s address space, allowing file I/O via normal memory access.
- Problems with transactional safety
- I/O stalls. Lack of async I/O
- Error handling is not modularized. [[SIGBUS Signals]]
- [[Performance]] issues, example: no compression and [[TLB Shootdowns]]
- See Pavlo's Are You Sure You Want to Use [[Memory-Mapped Files (MMAP)]] in Your [[Database Management Systems (DBMS)]]? (CIDR 2022)