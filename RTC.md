#notes
> [!info] Real-Time Clock (RTC)
> The Real-Time Clock is the internal counter of the bios, which ticks (generally) every millisecond from the first day of 1970. This clock is used to seed the [[System Clock]] at power on, specifically during the init system (runit/systemd/initrc etc...)

> [!warning] Reset of the RTC
> In case of a power failure, generally the CMOS battery being dead, the RTC will reset to a zero value. This can be then updated through the [[hwclock]] utility (specifically the `--systohc` flag)