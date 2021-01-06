# Intro
Guide on how to boot Ubuntu 18.04 from external hardrive (Live USB)  <br>
Also explains more about the process <br>

Some References:
* Original Guide [Create a USB stick](https://ubuntu.com/tutorials/create-a-usb-stick-on-windows)
* Original Guide [Try Ubuntu](https://ubuntu.com/tutorials/try-ubuntu-before-you-install)
* What is a [Live USB](https://en.wikipedia.org/wiki/Live_USB)
* Where to download [Ubuntu Desktop version](https://ubuntu.com/download/desktop) .
* What is [Rufus](https://rufus.ie/), [Github Rufus](https://github.com/pbatard/rufus)
* Guy that explained [MBR vs GPT](https://www.youtube.com/watch?v=Ch9f7i0hj90&t=1s) 

## Requirements
* A 4GB or larger USB stick/flash drive 
* Microsoft Windows XP or later
* Rufus, a free and open source USB stick writing tool
* An Ubuntu ISO file. 

## If you want persistent storage / Live USB 
If your goal is to readily use Ubuntu all the time.  \
Make sure to get a USB stick with **BOTH** good read + write speeds.  \
External Hard Drives shouldnt have this problem. 

# Booting using external harddrive
## Creating Ubuntu USB stick
### Rufus
Rufus is a utility that helps format and create bootable USB flash drives, [Link](https://rufus.ie/) to download.

### Honestly, follow Ubuntu's Guide
Honestly, follow the [Guide](https://ubuntu.com/tutorials/create-a-usb-stick-on-windows#1-overview) here, dunnid reinvent the wheel.

## WARNING / THINGS TO TAKE NOTE OF
### Select the right USB drive.
Ensure the drive selected in Rufus in the correct drive, or you'll end up formatting your laptop drive.

### MBR vs GPT // BIOS vs UEFI
In depth info watch [this explanation](https://www.youtube.com/watch?v=Ch9f7i0hj90&t=1s)   \
Basically:
* MBR with BIOS for compatibility
* GPT with UEFI for 2TB+ drives / GUI on bios 

### Persistent Partiton  
Set amount of Persistent storage space to set on the drive.  \
Basically its setting the amount of D: drive space.  

NOTE:
Do not set 100%, as this will leave no free space on your C: drive.  \
Making your system run very slow.  

## Switching to Ubuntu
Theres are 2 main ways to windows to boot from Ubuntu Drive.  \
Guides taken from [here](https://www.businessinsider.com/how-to-boot-from-usb-windows-10)

### 1. From Windows, Restart and boot from drive:
On windows:
* `Shift + click` restart.
* Wait for computer to restart.
* Advanced Startup Options screen appears.
* Choose "Use a device."
* Choose your USB device with Ubuntu.

### 2. Set boot priority on BIOS
When your computer boots:
* Ensure your Live USB is already connected.
* Press button to boot bios (Its different on different machines, google what your button is)
* For example, on Acer Predator 300 its `F2`
* Navigate to the section of boot priority.
* Set Live USB to have higher boot priority. (your computer will boot from Live USB first.)
* restart.

## Once Ubuntu Boots.
Click `Try Ubuntu`. (the other option will install Ubuntu on your system) \
Enjoy your Live USB Ubuntu!



