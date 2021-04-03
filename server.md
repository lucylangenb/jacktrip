# Running a Server
## Setting up port forwarding

These are mostly personal notes for myself. Only one person needs to run the server, while everyone else can connect to the server as clients.

In order for clients to connect to your server, you'll need to have port forwarding turned on. This basically means that other devices can see your public IP address and send packets of information to you. Specifically, JackTrip needs the port 4464 open.

Configuring port forwarding is, unfortunately, really different for each router. For most routers, you should be able to enter the router IP address into a new browser window to edit router settings. For Apple AirPort, you'll want to open AirPort Utility. Google is a much more helpful resource here than I will be because, again, how you set up port forwarding varies so much between devices.

For my future reference, here are some links I found useful:
- [Port forwarding on an Apple router](https://owlr.uservoice.com/knowledgebase/articles/875730-i-have-an-apple-router-how-do-i-set-up-port-forw)
- [ExpressVPN supports port forwarding - can be useful for hiding your public IP address](https://www.expressvpn.com/support/troubleshooting/router-app-port-forwarding/)

## Starting a server

With Jack running in the background, enter the command `jacktrip -s` in Terminal to enter server mode.

Type the following:
```
jacktrip -s -q 6 -n 1
```
- The q parameter is kind of like the buffer size - with a higher number, glitchiness is reduced, but latency increases. Remember that by typing `jacktrip` we can look at what default q is.
- The n parameter sets the number of channels (default 2) - fewer channels means less latency, but lower quality (non-stereo) audio. 
