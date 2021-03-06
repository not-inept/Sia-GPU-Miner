README

Miner v1.0.3
October 16, 2015
===============

The source code for the miner (and Sia as a whole) comes from Nebulous Labs,
check out their website for more info: https://siacoin.com/

This readme assumes you downloaded the latest release from the following link. It does not cover compiling from source:
	https://github.com/droghio/Sia-GPU-Miner/releases

Anyhow this is the latest Windows build of the Sia-GPU-Miner dubbed version v1.0.3.
Assuming everything unzipped correctly you should have the following five files.
	- README (That's me.)
	- LICENSE
	- sia-gpu-miner.exe
	- sia-gpu-miner.cl
	- libcurl.dll

If you are missing any of these files you have a problem,
try redownloading the binary from my github:
	https://github.com/droghio/Sia-GPU-Miner/releases

If you are still missing things (probably libcurl.dll) you might want to make sure your antivirus isn't
messing with your zip file. Norton is notorious for killing dlls without consent.

If the miner fails to load make sure you have the 2012 MS Redistributable installed:
	https://www.microsoft.com/en-us/download/details.aspx?id=30679

Other hints and tips:
	1. MAKE SURE YOU CHANGE THE INTENSITY!
		I upped the default intensity to 20 but make sure you
		change this if your care can take it! I'm talking about
		a 200+MH/s mining rate difference for a proper intensity value.
		I use an intensity of 27 on my 7970 and get about 770MH/s on a hefty overclock.

		To change this you'll need to launch the miner from a command prompt.
			a. Hit the Windows key start typing "cmd". 
			   You should see an app called Command Prompt

			b. After opening the command prompt type "cd " into the black window then 
			   click and drag the folder where the sia-gpu-miner.exe lives into the window.

			   You should see something like:
				C:\>cd C:\Users\John\Downloads\sia-gpu-miner.exe

			c. Press enter, then type "sia-gpu-miner.exe -I 27" where you replace the "27" with
				whatever intensity works best for your card. Too low and you aren't using
				your card's full potential, too high and you get diminishing returns.

	2. If you get an "HTTP error 400" make sure the Sia UI or siad is running AND you have unlocked your wallet.

	3. I compile the binary against AMD's OpenCL libs and this is a 64 bit binary meaning it won't run
	   on older machines. Even though I am using AMD's libs I have tested this program on a Nvidia 970
	   and got good hash rates (~1MH/s) so you should be fine using either brand of card.


If you have any questions concerns etc feel free to reach out to me via email or irc (freenode). In the mean time happy mining!
															- droghio