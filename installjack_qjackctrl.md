# Installing Jack
## OS X and Windows

Jack is essentially an audio patching software. Think about how a synth box works: you connect input and output sources via wires ("jacks") to create new sounds. Jack works the same way, but within your computer: it can route audio from one program to another.

Install Jack by visiting their website [here](https://jackaudio.org/downloads/).
- For Windows 7 and newer, install the 64 bit installer; for older operating systems, use the 32 bit installer.
- For Macs (10.12 and newer), use the Intel 64 bit installer. For older Macs, you'll need the Jack2 Binaries file, which is accessible through [an older version of the downloads page.](https://web.archive.org/web/20200808125552/https://jackaudio.org/downloads/)

You will need to restart your computer after installation. After you have done so, you will notice that Jack exists as a folder on your computer. JackPilot and qjackctl (Q Jack Control) both function as graphic interfaces for Jack; here, we'll use Q Jack Control. Note that, especially if you're using an older version of the download files, you might get an error message that the software isn't up-to-date; ignore this.

If, at any time, Q Jack Control isn't working for you, try following the [directions for using JackPilot instead.](https://github.com/lucylangenb/jacktrip/blob/master/installjack.md)

Upon opening Q Jack Control, you'll see one of the two windows shown below, depending on the version you downloaded. The buttons we care about are "Start" (though don't hit this yet), "Stop," "Patchbay," and "Setup." Ignore the other icons.

<p align="center">
  <img width="477" height="256" src="https://github.com/lucylangenb/jacktrip/blob/master/screencaps/qjackctl.png?raw=true">
</p>

Click "Setup." Depending on your version, the setup window can be somewhat overwhelming, but we only need to adjust a few settings.

<p align="center">
  <img width="1004.25" height="409.5" src="https://github.com/lucylangenb/jacktrip/blob/master/screencaps/qjackctl_setup.png?raw=true">
</p>

- __Sample Rate:__ This is how often your computer captures the sound you're making and converts it to binary code to be stored or transmitted (measured in samples per second, or Hz). For our purposes, 44100 Hz (44.1 kHz) is fine.
- __Frames/Period:__ This is how long it takes for your computer to process audio. A smaller value here can result in a loss of quality, but larger values can reintroduce latency. Musicians seem to like 128 samples here (not large enough to experience delays, but not too small that you start hearing glitches in transmitted audio).

After saving your changes in this setup window, try hitting the "Start" button in the small main window. Once things are up and running, feel free to open "Patchbay," although there's not much we can do with it yet. If you get a pop-up window ("Create patchbay definition as a snapshot of all actual client connections?"), hit "No" to make sure we'll be able to make the necessary connections later.

<p align="center">
  <img width="670" height="350" src="https://github.com/lucylangenb/jacktrip/blob/master/screencaps/qjackctl_initialpatchbay.png?raw=true">
</p>

This window is essentially your computer's synth box. Here, you can see boxes where input and output channels will be shown so that we can virtually connect (patch) them. We'll come back to this window to do some patching later - for example, we'll add Jacktrip (which can send audio elsewhere) as an input channel to route our audio to another musician's computer.

Next, we need to install JackTrip. Installation is a little trickier on Windows, so I've made separate guides for [OS X](https://github.com/lucylangenb/jacktrip/blob/master/installjacktrip_osx.md#installing-jacktrip) and Windows, both of which can also be accessed from the main page.
