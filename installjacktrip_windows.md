# Installing JackTrip
## Windows

Jack routes audio between programs within your computer, but we need JackTrip to direct audio between multiple different computers. However, before we can deal with JackTrip, you'll likely need to download an ASIO driver, which essentially directly connects software to your computer's sound card, bypassing default Windows audio drivers (this is the step that makes Windows installation more complex than installation for Macs). You can find the download on the ASIO4All site [here](https://www.asio4all.org/), or via specific download links:
- For Windows 10 and newer, use the newest [beta software.](https://www.asio4all.org/downloads_11/ASIO4ALL_2_15(Beta1)_English.exe)
- For older versions of Windows, use the [2017 release.](https://www.asio4all.org/downloads_11/ASIO4ALL_2_14_English.exe)

Double-click the .exe file and follow installation instructions. When prompted with the __Choose Components__ section of the installer, make sure to allow offline settings. This will allow you to continue to adjust ASIO settings even while JackTrip isn't open.

You'll also want to make sure to adjust the buffer size. Remember "Frames/Period" from Jack settings? This is the same deal. Make sure these numbers match (128 samples).

Before finishing ASIO setup, we'll need to download and install JackTrip. Download jacktrip-1.1-osx.zip, located in the Assets drop-down menu, from the developers' [GitHub repository.](https://github.com/jacktrip/jacktrip/releases/tag/v1.1) Although this may seem like a weird place to download files from, these Stanford researchers use GitHub to keep track of and update their work, and this is a safe download.

You'll notice that the zip file contains INSTALL.txt - this is basically a more techincal version of this guide. Feel free to use it if you prefer.

Open up Terminal (which you can reach from Launchpad by opening __Other → Terminal__). We'll be running code just like any other program on your computer does, but without the easy-to-use graphic interface that we're used to computer programs having - i.e. we'll have to type (or copy and paste) code instead of clicking buttons. It's worth getting familiar with Terminal:

<p align="center">
  <img width="324" height="106" src="https://github.com/lucylangenb/jacktrip/blob/master/screencaps/osx_terminal.png?raw=true">
</p>

- __bash__ is what's known as a command-line interpreter. Basically, instead of the graphical user interface (GUI) that non-programmers are used to, this is a program that manages a text-based interface. 
- __MacBook-Air-19__ is the name of the device I'm using.
- __LucyR$__ is the directory I'm currently in. Think of it as where I am currently positioned within my computer's library.

Enter the following lines of code one at a time. Their functions are explained below.
```
cd Downloads/jacktrip/bin
sudo cp jacktrip /usr/local/bin/
sudo chmod 755 /usr/local/bin/jacktrip


```
- The "cd" in the first command stands for change directory. This command relocates you to the binary folder within the JackTrip folder. Make sure you're formatting your directory commands to exactly match the syntax of the folders within your computer (capitalize Downloads, etc).
- "sudo" in the second line means "as an administrator." In normal English, then, the second command means "with administrator privileges, copy jacktrip into the folder I want." You're making a copy of the executable file in a place that your computer expects to find it so that this runs properly. __You'll have to enter your password__, but this is fine; you need to give administrator privileges briefly to allow Terminal to make a copy of this file.
- The third line of code modifies permissions on the jacktrip file so you'll be able to run it properly.

Other useful commands to know:
- `ls` lists the contents of the current directory.
- `cd` without any additional arguments will redirect you to the home directory.
- `pwd` shows you the "present working directory" (the full path of the directory you're in).

Open Terminal again (⌘T for a new tab, ⌘N for a new window) to make sure your changes went through. Type `jacktrip` and hit enter (doesn't matter which directory you're in) to run the program. You'll then see a lot of text describing how to make JackTrip work:

<p align="center">
  <img width="644" height="510" src="https://github.com/lucylangenb/jacktrip/blob/master/screencaps/osx_jacktripcommands.png?raw=true">
</p>

Because JackTrip is command-line, we'll need to pass arguments to the program (typing in commands) to tell the program what we want it to do. If we're ready to join a server, continue on to the [Running JackTrip guide.](https://github.com/lucylangenb/jacktrip/blob/master/run_osx.md#running-jack-and-jacktrip)
