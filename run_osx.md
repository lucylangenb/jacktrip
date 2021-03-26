# Running Jack and JackTrip
## Connecting to a server

Now that we've installed Jack and JackTrip, we can finally connect to a server! First, make sure Jack is running (hit the "Start" button). Then, open up a new Terminal window. If you need a refresher on the types of arguments you can pass to JackTrip, type `jacktrip` to generate a list of helpful commands.

To run JackTrip in client mode, enter the following command (though, instead of ipAddress, you would enter the IP address of the person running the server).
```
jacktrip -c ipAddress
```
That's it! You should be connected to the server. Don't worry about the "UDP waiting too long" message. If you're having trouble sending and receiving audio, this is a message worth looking into, but in most cases it is meaningless.

If you're having problems:
- Check to make sure that the buffer size in Jack is the same between all users. Stick to 128 for simplicity; if you want to explore other sizes (64, 256), you'll have to close Jack and JackTrip (use ⌘C in Terminal to stop JackTrip), adjust this preference, and run the programs again.


