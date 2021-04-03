# ASIO Driver Installation

If you use a Windows device, congratulations! You probably need to install one of these in addition to Jack and JackTrip. The folks at Stanford have a pretty comprehensive [guide](https://ccrma.stanford.edu/software/jacktrip/windows/index.html) on how to install one of these and connect it to Jack and JackTrip, but in case that isn't clear enough, this is some extra guidance. __However, I would encourage you to read through the Stanford page first - I have a Mac, and the Stanford folks know much more about Windows devices than I do.__ After installing your ASIO driver, [return to my Jack installation guide](https://github.com/lucylangenb/jacktrip/blob/master/installjack_qjackctrl.md#installing-jack) - Stanford uses slightly different settings than I do.

An ASIO driver essentially directly connects software to your computer's sound card, bypassing default Windows audio drivers (this is the step that makes Windows installation more complex than installation for Macs). You can find the download on the ASIO4All site [here](https://www.asio4all.org/), or via specific download links:
- For Windows 10 and newer, use the newest [beta software.](https://www.asio4all.org/downloads_11/ASIO4ALL_2_15(Beta1)_English.exe)
- For older versions of Windows, use the [2017 release.](https://www.asio4all.org/downloads_11/ASIO4ALL_2_14_English.exe)

Double-click the .exe file and follow installation instructions. When prompted with the __Choose Components__ section of the installer, make sure to allow offline settings. This will allow you to continue to adjust ASIO settings even while JackTrip isn't open.

You'll also want to make sure to adjust the buffer size. Identical to "Frames/Period" in Jack settings, this is how long it takes your computer to process audio. Make sure the value here matches whatever you have or plan to have in Jack (128 samples).


