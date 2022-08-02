# Edit hosts file

The hosts file is a system file on a device that lets you map specific domain names to an IP address. If you want 
to add new entries to the hosts file, you’ll need the IP address of the server that you want to map a hostname to.

    XXX.XXX.XXX.XXX some.domain.name 

The hosts file lets you override DNS entries for any domain name. There are lists of common ad networks and 
tracking servers available online which you can use to keep an up-to-date list of sites to block. Blocking is achieved 
by setting the IP address of the ad networks to a loopback address like 127.0.0.1 which will not return anything. 
There are lists of common ad networks and tracking servers available online which you can use to keep an up-to-date 
list of sites to block. 

If your device is infected with malware, then your hosts file may be compromised to included unknown entries for known 
domain names. *That* is NOT the IP address of your bank! This type of DNS attack is known as DNS pharming, and checking 
your `hosts` file can uncover potential infection.

## Windows

To edit the hosts file (`C:\Windows\System32\Drivers\etc\hosts`) on Windows, you will need Administrator access. 

* Right-click on your text editor’s icon (for example Notepad++) and choose //Run as administrator//.
* Go to File → Open in the text editor and navigate to `C:\Windows\System32\drivers\etc\`
* From the list, click on the hosts file and choose Open
* Add as many new entries as needed
