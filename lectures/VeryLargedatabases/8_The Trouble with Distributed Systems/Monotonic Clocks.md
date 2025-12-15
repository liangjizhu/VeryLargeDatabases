A clock that never goes backward, even if the system’s time-of-day clock is adjusted. It only measures elapsed time, not real-world calendar time.
- Suitable for measuring a duration
- clock_gettime(CLOCK_MONOTONIC)
- System.nanoTime()
- Used for measurements
- Cannot be compared between computers