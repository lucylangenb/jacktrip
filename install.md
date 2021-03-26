# Installing Jack and Jacktrip

## Installing Jack

Jack is essentially an audio patching software. Think about how a synth box works: you connect input and output sources via wires ("jacks") to create new sounds. Jack works the same way, but within your computer: it can route audio from one program to another.

To download the most recent version of Jack for Windows or OS X, [visit the Jack website.](https://jackaudio.org/downloads/)
(As of 8/21/20, the Windows and OS X software links are no longer available on this site. Check out [this Wayback link](https://web.archive.org/web/20200808125552/https://jackaudio.org/downloads/) for an older version of this page with download links.)
- For Windows 7 and newer, download the 64 bit installer. For older computers, you'll want the 32 bit installer.
- For OS X, download the Jack2 Binaries file.

You will need to restart your computer after installation. After you have done so, you will notice that Jack exists as a folder on your computer. JackPilot and qjackctl (Q Jack Control) both function as graphic interfaces for Jack; here, we'll use JackPilot.

Upon opening JackPilot, you'll be navigated to a settings window (you can get here again by selecting __JackPilot → Preferences__ in OS X):

<p align="center">
  <img width="396" height="566" src="https://github.com/lucylangenb/jacktrip/blob/master/screencaps/jackpilot_preferences.png?raw=true">
</p>

You'll want to pay attention to a few features:
- __Input/Output Device:__ Especially if you have an external mic that you're using (recommended, but not required), make sure these are correct.
- __Sample Rate:__ This is how often your computer captures the sound you're making and converts it to binary code to be stored or transmitted (measured in samples per second, or Hz). For our purposes, 44100 Hz (44.1 kHz) is fine.
- __Buffer Size:__ This is how long it takes for your computer to process audio. Smaller buffer sizes can result in a loss of quality, but larger buffer sizes can reintroduce latency. Musicians seem to like 128 here (not large enough to experience delays, but not too small that you start hearing glitches in transmitted audio).
- __Interface Input/Output Channels:__ These should automatically match your input/output device, but it's worth checking to make sure. My Apple headphones have two input and two output channels, for example.
- __Virtual Input/Output Channels:__ Again, these should be correct (and should match the interface in/out channels), but check to make sure.

In the small main JackPilot window, try hitting the start button. This will start Jack on your computer - nothing's really happening because we haven't told Jack what we want it to do with our audio. Click the now-available "Routing" button to access the Connections Manager.

The Connections Manager window is essentially your computer's synth box. Here, you can see all available input (capture) and output (playback) channels and virtually connect (patch) them. We'll come back to this window to do some patching later - for example, we'll add Jacktrip (which can send audio elsewhere) as an input channel to route our audio to another musician's computer.

