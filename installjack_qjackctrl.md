# Installing Jack
## OS X and Windows

Jack is essentially an audio patching software. Think about how a synth box works: you connect input and output sources via wires ("jacks") to create new sounds. Jack works the same way, but within your computer: it can route audio from one program to another.

Install Jack by visiting their website [here](https://jackaudio.org/downloads/).
- For Windows 7 and newer, install the 64 bit installer; for older operating systems, use the 32 bit installer.
- For Macs (10.12 and newer), use the Intel 64 bit installer. For older Macs, you'll need the Jack2 Binaries file, which is accessible through [an older version of the downloads page](https://web.archive.org/web/20200808125552/https://jackaudio.org/downloads/).

You will need to restart your computer after installation. After you have done so, you will notice that Jack exists as a folder on your computer. JackPilot and qjackctl (Q Jack Control) both function as graphic interfaces for Jack; here, we'll use Q Jack Control. Note that, especially if you're using an older version of the download files, you might get an error message that the software isn't up-to-date; ignore this.

Upon opening Q Jack Control, you'll see one of the two windows shown below, depending on the version you downloaded. The buttons we care about are "Start" (though don't hit this yet), "Stop," "Patchbay," and "Setup." Ignore the other icons.

(qjackctl)

Click "Setup." Depending on your version, the setup window can be somewhat overwhelming, but we only need to adjust a few settings.

(qjackctl_setup)

- __Sample Rate:__ This is how often your computer captures the sound you're making and converts it to binary code to be stored or transmitted (measured in samples per second, or Hz). For our purposes, 44100 Hz (44.1 kHz) is fine.
- __Frames/Period:__ This is how long it takes for your computer to process audio. A smaller value here can result in a loss of quality, but larger values can reintroduce latency. Musicians seem to like 128 samples here (not large enough to experience delays, but not too small that you start hearing glitches in transmitted audio).




