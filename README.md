# Voron-Printer-Guide
Walk through guide relating most of the things Voron c:

_________________________________________________________
## Setting up Klipper, Moonraker, and Mainsail/Fluidd
Probably the easiest way to manage and download these is through [Kiauh](https://github.com/dw-0/kiauh). 
Here, we'll take a quick stroll through the installation and setup for the minimal required softwares to get your printer running.

### Download/install Kiauh
Get or update git:
```
sudo apt-get update && sudo apt-get install git -y
```
Then, download Kiauh itself:
```
cd ~ && git clone https://github.com/dw-0/kiauh.git
```
Now thats Kiauh is installed, you'll need to memorize one command:
```
./kiauh/kiauh.sh
```
Enter it now, this is used to acces the Kiauh menu.
You can decline all of the update requests.

Now that Kiauh is installed, we can start downloading Klipper itself.

The order of downloading is Klipper, Moonraker, Mainsail/Fluidd. This is important since it can sometimes show errors (atleast in my experience).
_________________________________________________________
### Download/install Klipper 🐟
Navigating through Kiauh is done with number (you probably already figured that out). To install, choose "Install" on the main menu.

From the install menu, download Klipper.

*During the download, it will ask how many instances you want to set up. 1 should be the default.*

Installing Klipper may take a while depending on internet speeds and other factors. After it's installed, you should be directed back to the install menu, if you didn't get any errors, proceed to downloading Moonraker.
_________________________________________________________
### Download/install Moonraker 🌒
From the install menu, download Moonraker.

*During the download, it will ask for different parameters. Unless you know what you're doing, it's recommended to keep them at default.*

**If you made more then 1 instance of klipper, you'll have to download Moonraker for all of the instances**

After the installation, you'll be redirected to the install menu, if no errors showed up, proceed to the next step. 
_________________________________________________________
<ins>For the next part you'll need to choose what end you want to use: Mainsail or Fluidd. There isn't a better or worse option.</ins> To prevent issues, only get one of them.
_________________________________________________________
### Download/install Mainsail ⛵
Through the install menu, download Mainsail

*Leave all of the parameters at default unless you know what you're doing*

### Download/install Fluidd 🌊
The steps for downloading Fluidd are the same as for Mainsail.
_________________________________________________________
## Flash Klipper and Find Board IDs
**This part is important**

*If you have a CAN toohead board, you'll need to follow [this guide](https://canbus.esoterical.online/) for setting up CANBus. I personally followed it and it does work (as of Feb. 2025). Reconnect back with us at "[Access the Printer](https://github.com/Suzu0071/General-Guide-for-Vorons/tree/main?tab=readme-ov-file#access-the-printer)" section*

*If you don't have a CAN toolhead board or are using a USB one, then you can stay on this page.*
_________________________________________________________
### Flashing the Board
Because flasing board is such a big section, I decided to move it to a different doc. --> ![Click Me!](https://github.com/Suzu0071/General-Guide-for-Vorons/blob/main/BoardFlash.md)
_________________________________________________________
## Access the Printer
Remember the IP address you used to SSH into your device? You'll need it again!

Paste it into the search bar of your browser and enter:
![](https://github.com/Suzu0071/General-Guide-for-Vorons/blob/main/Images/IP-example.png)

Mine is 192.168.0.19, but yours is probably different. 

You will find yourself on the main screen of the printer, this is where you'll be spending the most time from now on.

![](https://github.com/Suzu0071/General-Guide-for-Vorons/blob/main/Images/Mainsail-Main-Example.png)

I have Crowsnest and Spoolman installed but you can ignore that for now. I'll be showing everything on Mainsail, but Fluidd should be very similar.
_________________________________________________________
On the left, click "MACHINE", you'll be transported to the config and file section of the printer.

![](https://github.com/Suzu0071/General-Guide-for-Vorons/blob/main/Images/Mainsail-Machine-Example.png)

<sup>Mine has a bunch of stuff already x:</sup>

First, make a printer.cfg file:
1. Click the little "Create File" button
2. wadf
