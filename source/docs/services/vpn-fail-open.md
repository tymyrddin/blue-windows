# Make a VPN killswitch using routes

If you simply add a VPN using common instructions, it generally "fails open". That means, if the VPN breaks down, 
because the connection is interrupted, traffic will be sent without the VPN. It is much safer when it "fails closed", 
meaning that when the VPN connection breaks down, the whole internet connection must be down as long as the VPN 
connection is not restored. If your [chosen VPN](vpn.md) does not include being able to 
set a kill switch, you can use routes as a fail-safe mechanism:

Make sure you’re connected to the OpenVPN server:

* Run the Command Prompt with admin rights.
* Delete the default route when the OpenVPN connection is established.

```text
> route delete 0.0.0.0
```

Now the default routing method is deleted, making VPN the only access method to the internet. Your internet 
connection will be cut off when VPN is inaccessible. The operating system will remain stasis until it can access that 
route again. Note that this state is ot persistent. If the router reboots or the adapter is disabled, the settings 
will be taken to a default state.

To manually restore the default settings:

* Go to Control Panel -> Network and Internet -> Network and Sharing Center.
* Click Change adapter settings.
* Disable and then enable it again.