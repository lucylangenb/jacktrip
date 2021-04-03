# Installing JackTrip
## Windows

Jack routes audio between programs within your computer, but we need JackTrip to direct audio between multiple different computers. To download and install JackTrip, check out the [Stanford page](), or visit these direct links:
- [Windows 10 and newer](https://ccrma.stanford.edu/software/jacktrip/windows/jacktrip.exe)
- [Older versions of Windows](https://ccrma.stanford.edu/software/jacktrip/windows/1.2.1/jacktrip.exe)

Open up Command Prompt (which you can access by right-clicking on the home button). JackTrip does not have a graphic interface, so we'll need to enter a few basic commands to get it running. However, most importantly, __JackTrip can only be run when you, the user, are within the same folder as JackTrip is.__ This means that every time we run JackTrip, we will first have to type the following line of code (or its equivalent):

```
cd Downloads
```
The "cd" stands for change directory. This command relocates you to the Downloads folder. Make sure you're formatting your directory commands to exactly match the syntax of the folders within your computer (capitalize Downloads, etc). If you're not sure where JackTrip is located, find the file in Files, then drag the file into Command Prompt. This will show you the directory location of JackTrip - just delete the "jacktrip.exe" part at the end of the location to ensure that you are relocated to the folder within which JackTrip resides.

Type `jacktrip` and hit enter to generate a list of the arguments we can pass to JackTrip (in other words, the commands we can send it). 

<p align="center">
  <img width="644" height="510" src="https://github.com/lucylangenb/jacktrip/blob/master/screencaps/osx_jacktripcommands.png?raw=true">
</p>

Because JackTrip is command-line, we'll need to pass arguments to the program to tell the program what we want it to do. If we're ready to join a server, continue on to the [Running JackTrip guide.](https://github.com/lucylangenb/jacktrip/blob/master/run_osx.md#running-jack-and-jacktrip)
