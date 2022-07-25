# Introduction

There are many types of devices and mechanisms within the security environment to provide a layered approach of defense. 
This is so that if an attacker is able to bypass one layer, another layer stands in the way to protect the network. 
Two of the most popular and significant tools used to secure networks are firewalls and intrusion detection systems. 

## Choosing a firewall for a Windows PC

With a firewall, you can:

* Log hosts scanning services that aren't running.
* Limit the services that applications can connect to.
* Segregate the local network into trust segments (Local Area Network (LAN), DeMilitarised Zone (DMZ), and Internet).
* Redirect ports to the hosts providing the service (Network address translation (NAT)).

Windows comes with a [built-in firewall](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-firewall/windows-firewall-with-advanced-security) in Windows 10, but this firewall may be turned off by default. 

Turn it on via Settings:

* Under Windows Settings section, click Update & Security. 
* Select Windows Defender and then click Open Windows Defender Security Center. 
* Choose Firewall & network protection and choose a network profile. 
* Under the Windows Defender Firewall section, switch Off to On.
* In order to allow a specific application to pass through your Windows Firewall, you have to add it to the list of other permitted applications. You can do this by clicking Allow an app or feature through Windows Defender Firewall.

If you’d like to be more secure, install a firewall (none of which offer exploit attack protection, by the way).

* [ZoneAlarm](https://www.zonealarm.com/software/free-firewall)
* [Comodo](https://personalfirewall.comodo.com/)
* [TinyWall](https://tinywall.pados.hu/)

## Choosing a HIDS for a Windows PC

Most of the [HIDS tools for Windows](ids.md) are EventLog Analyzers.

## Related attack trees

* [Scanning](attack-trees:docs/scanning/README)
* [Malware](attack-trees:docs/malware/README)
* [System](attack-trees:docs/system/README)
* [Network](attack-trees:docs/network/README)