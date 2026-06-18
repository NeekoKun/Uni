#notes 
> [!info] Network Time Protocol (NTP)
> The Network Time Protocol is used by devices to sync the time across internet. It usually runs on [[UDP]] port 123. In case this is blocked, there exist a multitude of alternatives supported by various NTP daemons

### Alternatives
---
In case [[UDP]] 123 is blocked, stock [[NTP]] will not work properly. In these cases:
- Check if the [[ISP]] / [[DHCP]] protocol handed a custom [[NTP]] server address
- Utilize [[NTS]], which could work as it initializes the connection on [[UDP]] 4460, although the actual data exchange is still performed on [[UDP]] 123
- Customize the [[UDP]] port on a proprietary [[NTP]] server, accessed through a [[VPN]] or similar
- Utilize [[htpdate]] to sync through the `Date: ` field in an [[HTTP]]/[[HTTPS]] header when [[NTP]] fails, as a backup