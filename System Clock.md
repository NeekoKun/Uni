c#notes 
> [!info] System Clock
> The system clock is a kernel-level counter seeded at init from the [[RTC]]. This clock is in turned used by the processes such as [[SSL]] and `date` as the clock of the machine.

> [!info] Clock synchronization
> To synchronize clocks across the internet, the [[NTP]] protocol is used. This runs on [[UDP]] 123 and is usually managed by daemon services such as:
> - [[Chrony]]
> - [[openntpd]] ==(deprecated)==