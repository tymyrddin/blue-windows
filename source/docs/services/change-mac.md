# Change MAC address

A MAC address identifies the device connected to a network and allows the network to track, restrict or allow access 
based on it. Routers identify and assign static IP addresses based on the MAC addresses of devices. Before you try to 
change the MAC address, you need to know the value that you want to use.

Set the 2's place bit (the "locally administered" bit) in the first byte, to differentiate it from a guaranteed 
globally unique MAC address. Usually the first three bytes an unicast MAC address is an 
"Organizationally Unique Identifier" (OUI) that the IEEE assigned to the manufacturer of your Ethernet device. 
Manufacturers are required to make sure they keep the last 3 bytes unique. 

Avoiding all of that knowledge, the [MAC address generator tool](https://miniwebtool.com/mac-address-generator/) can 
generate a valid address for you.

## Device Manager

* In the Device Manager window, click the arrow next to Network adapters.
* Right-click the adapter for the network card that you want to change.
* Choose Properties from the menu.
* Select the Advanced tab. 
* Select Network Address in the Property displayed list.
* Type the new MAC address value on the right side. 
* Press the OK button.

## Control Panel

* In the Control Panel window, search for "network connections" and choose "View network connections" in the results.
* Right-click on the network connection you want to change. 
* Choose Properties from the menu.
* In the Properties window, click the Configure button.
* In the new Properties window that pops up, select the Advanced tab.
* Select Network Address in the Property displayed list.
* Type the new MAC address value on the right side. 
* Press the OK button.
