# Configs
## Optimizations
> [!info] Watchdog
> ```watchdog ``` is a service which automatically reboots the system with OS hangs. On a consumer pc, it can be disabled with
> ```sh
> GRUB_CMDLINE_LINUX_DEFAUL = "... nowatchdog"
> ```
> in `/etc/default/grub`, and
> ```sh
> echo "blacklist iTCO_wdt" | sudo tee /etc/modprobe.d/nowatchdog.conf
> ```
> to prevent module loading entirely