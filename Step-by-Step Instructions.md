# Step-by-Step Instructions

## November 2023 Update
This project has been massively overhauled since its inception in 2018. The 2018 instruction set contained a bunch of workarounds and custom python scripting to get it to work. 
The team at Raspberry Pi have since created a native emulator which makes this project nearly turn-key. To make this more accessible to others, I have updated the instructions to reflect the new process. You will find all instructions necessary to build this for yourself on this page.

## Step 1: Prepping Pi
  1. Head over to [Raspberry Pi Downloads](https://www.raspberrypi.com/software/) and download the latest version of the Raspberry Pi Imager for your machine.<br>
  2. Once downloaded, open up the imager and select the correct version of Raspberry Pi for your build. For Operating System, select 'RetroPie' and the appropriate version for your Pi. Finally, for storage, choose your SD card slot.<br>
  3. Proceed to overwrite and install the new software<br>
  4. (optional) If you would like to primarily run widescreen games (such as SNES games) and also want a horizontal screen orientation, you should skip this step. If you are planning to primarily run vertical or vertical-scrolling games (such as Pacman, Raiden, etc) then I would highly recommend rotating your screen. To do that:
      1. Open up your file explorer
      2. Click into your SD drive
      3. Open the config.txt file
      4. At the bottom of the file, add a new line and type (excluding the quotations) "display_rotate=1"
      5. Save
  5. Eject your SD Card, plug it into your Raspberry Pi

## Step 2: Prepping USB Drive
  1. Format your USB drive to either exFAT or FAT32. To do this:
      1. Open Disk Utility (Mac) or Disk Management (PC)
      2. Select the 'erase' option
      3. In the erase configuration, rename your drive (anything you want,) select either exFAT or FAT32, and press go
  2. Once configured, open the USB drive up in file explorer
  3. Create a new folder. Name it (excluding quotations) "retropie-mount"

## Step 3: Loading ROMs onto your USB drive
  1. This is the only part you will need to figure out on your own. ROMs = Games. Now, you can purchase these ROMs from any number of sellers online. Some people will pirate them. You're an adult. DYOR (Reddit obv a great resource for this,) gather your roms and continue on...
  2. Once you have your roms downloaded, you will probably need to unzip/extract them.
  3. Once you have the individual file folders for each of your ROMs, copy/paste (move) them over to the retropie-mount folder we made earlier
  4. Once copy is complete, eject the drive, plug it into your Raspberry Pi

## Step 4: Assembly
  1. 

