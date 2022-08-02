# Renew IP lease 

A DHCP client can on occasion send information in DHCP requests: hostname, MAC address, operating system, and DHCP 
version. All operating systems provide their most recent IP address to the DHCP server. 
If you [change your MAC address](change-mac.md) to minimise risk, best to also renew the IP leases on the 
router.

## Windows

Using a `/renew switch` (This command won't work if the computer is configured to use a static IP address):

```
C:\>ipconfig /renew
```
