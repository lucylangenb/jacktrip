# Running Jack and JackTrip
## Connecting to a server

Now that we've installed Jack and JackTrip, we can finally connect to a server! First, make sure Jack is running (hit the "Start" button). Then, open up a new Terminal window. If you need a refresher on the types of arguments you can pass to JackTrip, type `jacktrip` to generate a list of helpful commands.

To run JackTrip in client mode, enter the following command (though, instead of ipAddress, you would enter the IP address of the person running the server).
```
jacktrip -c ipAddress -q 6 -n 1
```
That's it! You should be connected to the server. The "q" and "n" arguments are adjusting audio input/transfer settings to better optimize latency and quality; these must match the settings of the server.

Don't worry about the "UDP waiting too long" message. If you're having trouble sending and receiving audio, this is a message worth looking into, but in most cases it is meaningless.

If you're having problems:
- Check to make sure that the buffer size in Jack is the same between all users. Stick to 128 for simplicity; if you want to explore other sizes (64, 256), you'll have to close Jack and JackTrip (use control-C in Terminal to stop JackTrip), adjust this preference, and run the programs again.
- Check to make sure your q and n arguments (if applicable) match the server's.

## Patching in Jack

In JackPilot, hit the "Routing" button to open the Connections Manager. Because you have JackTrip running, you'll see JackTrip as input ("Send Ports") and output ("Receive Ports") options. Try selecting one of your system input options; if you are connected to a server correctly, the corresponding JackTrip output will appear in red.

<p align="center">
  <img width="587" height="435" src="https://github.com/lucylangenb/jacktrip/blob/master/screencaps/jackpilot_connectionswhilerunning.png?raw=true">
</p>

Because I have "capture_1" selected, for example, JackTrip's "send_1" appears in red. 

To create additional connections (virtually plugging cables into input and output channels on your imaginary synth box), select the input you want, then double-click the output you want to connect it to. You can undo connections the same way (if a connection is already present, select the input, then double-click the corresponding output). As far as I can tell, it doesn't matter too much which "capture" inputs are routed to JackTrip's "send" output(s), for our purposes, but you do want to make sure you route both "playback" outputs to JackTrip's "receive" input(s). On most computers, "playback_1" corresponds to your left headphone/earbud, while "playback_2" corresponds to your right headphone/earbud. 

