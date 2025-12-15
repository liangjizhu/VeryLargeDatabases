A physical clock on a computer that tracks real-world calendar time—the current date and time (e.g., 2025-03-10 14:32:05). It is what your operating system shows when you ask for the current time.
In [[Distributed System]], time-of-day clocks are considered unreliable for ordering events because they can drift, jump and differ between machines.
- Wall-clock time
- System.currentTimeMillis()
- clock_gettime(CLOCK_REALTIME)