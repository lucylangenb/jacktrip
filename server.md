# Running a Server
## Setting up port forwarding

These are mostly personal notes for myself. Only one person needs to run the server, while everyone else can connect to the server as clients.

In order for clients to connect to your server, you'll need to have port forwarding turned on. This basically means that other devices can see your public IP address and send packets of information to you. Specifically, JackTrip needs the ports 4464-4485 open.

With Jack running in the background, enter the command `jacktrip -s` in Terminal to enter server mode.

Type the following:
```
jacktrip -s -q 6 -n 1
```
- The q parameter is kind of like the buffer size - with a higher number, glitchiness is reduced, but latency increases. Remember that by typing `jacktrip` we can look at what default q is.
- The n parameter sets the number of channels (default 2) - fewer channels means less latency, but lower quality (non-stereo) audio. 
