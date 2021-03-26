# Installing JackTrip
## OS X

Jack routes audio between programs within your computer, but we need JackTrip to direct audio between multiple different computers. Download jacktrip-1.1-osx.zip, located in the Assets drop-down menu, from the developers' [GitHub repository.](https://github.com/jacktrip/jacktrip/releases/tag/v1.1) Although this may seem like a weird place to download files from, these Stanford researchers use GitHub to keep track of and update their work, and this is a safe download.

You'll notice that the zip file contains INSTALL.txt - this is basically a much more dense, technical version of this guide. Feel free to use it if you prefer, but I found it tough to digest.

Open up Terminal (which you can reach from Launchpad by opening __Other → Terminal__). We'll be running code just like any other program on your computer does, but without the easy-to-use graphic interface that we're used to computer programs having - i.e. we'll have to type (or copy and paste) code instead of clicking buttons.

(image here)

It's worth getting familiar with this window:
- __bash__ is what's known as a command-line interpreter. Basically, instead of the graphical user interface (GUI) that non-programmers are used to, this is a program that manages a text-based interface. 
- __MacBook-Air-19__ is the name of the device I'm using.
- __LucyR$__ is the directory I'm currently in (which we know because of the tilde, ~, in front of it). Think of it as where I am currently positioned within my computer's library.

Enter the following lines of code, which are explained below:
```
cd Downloads/jacktrip
```
- `cd Downloads/jacktrip`: the "cd" stands for current domain. This command relocates you to the JackTrip folder.

