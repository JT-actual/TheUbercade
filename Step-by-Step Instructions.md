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
  1. This is the only part you will need to figure out on your own. ROMs = Games. Now, you can purchase these ROMs from any number of sellers online. Some people will pirate them. You're an adult. DYOR (Reddit a great resource for this,) gather your roms and continue on...
  2. Once you have your roms downloaded, you will likely need to unzip/extract them.
  3. Once you have the individual file folders for each of your ROMs, copy/paste (move) them over to the retropie-mount folder we made earlier
  4. Once copy is complete, eject the drive, plug it into your Raspberry Pi

## Step 4: Assembly
This part is relatively self-explanatory, but for sake of completeness, we will cover. Depending on your setup, I'd probably recommend making some sort of mounting plate. I took a thin piece of sheet metal and bolted it in place using the VESA mount on the back of the monitor. You could also just stick the RPI to the monitor using some 3M double sided tape (assuming you had a case for your RPI, ofc.)

After that, hook it all up. You should have 1x HDMI, 2x SNES controllers, 2x power connectors (one for the monitor and one for RPI)

Note on power connectors: I might recommend that you grab a DC inverter with two AC outlets for this install, depending on your ride. When I first set this up, I had a single outlet inverter, which I ran my monitor to (so, monitor power cable > DC inverter > car) which left me to run my RPI straight off a USB charging port in my center console. I sometimes had power issues (RPI randomly shutting off/lagging) that I believe were caused by that setup, so if you're in this for the long haul, its certainly worth the relatively small investment.

## Step 5: Boot it up!
Look at you, hot shot. We're just about done! There's really not much else to do here. Once you boot up your RPI, it should take you to a controller configuration screen. Make sure you assign all of the buttons properly.

Right after that, it will take you to the home screen where you should find all of the games you loaded onto the USB drive (if not, or if you get an error about not being able to find the path or something like that, try to start this process over from step 1. If it's still an issue, your SD card may be corrupted, which happens quite a lot. In that event you'll want to replace the card.)

Assuming all is fine, I'd recommend going into Settings > Scraper and use one of the scrapers to pull in game data (like the original case artwork, etc) just to make things look prettier in the UI.

## Final note

For those professional drivers that made it through the install, I would love to hear how this is working out for you. I found it brought immense joy to both my passengers and myself and I was able to significantly increase my earnings with it. Hope it brings you the same.

Cheers!

