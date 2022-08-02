# Use a Tor proxy

## Tor proxy

Install:

    $ sudo apt update
    $ sudo apt install tor

Check it is installed: 

    $ tor --version
    Tor version 0.4.6.9.

Get your IP address:

    $ curl ifconfig.me; echo
    [IP address]

Run the same command but preface it with torsocks. The command is now run through the tor client instead:

    $ torsocks curl ifconfig.me; echo
    [Some Tor IP address]

To use the Tor network by default for shell commands, torify your shell with this command:

    $ source torsocks on
    Tor mode activated. Every command will be torified for this shell.

Test with (must now be []):

    $ curl ifconfig.me; echo
    [Some Tor IP address]

## Notes

* If a government makes their own national internet, or routes traffic through specific servers to use deep packet inspection (DPI), running Tor may not provide security if the government is able to see the entire path. 
* Sometimes the Tor network is censored, and clients can't connect to it. An increasing number of censoring countries are using Deep Packet Inspection (DPI) to classify Internet traffic flows by protocol. While Tor uses bridge relays to get around a censor that blocks by IP address, the censor can use DPI to recognize and filter Tor traffic flows even when they connect to unexpected IP addresses. With pluggable transports, censorship against Tor can be bypassed.
* Not only that. If an attacker can see your traffic, and can see the website you're visiting, even with a path outside the adversary's control - they will still be able to correlate the traffic and learn you are visiting the website.
* If the same connection (the same set of relays) were to be used for a longer period of time a Tor connection could be vulnerable to statistical analysis, which is why the client software changes the entry node every ten minutes.

