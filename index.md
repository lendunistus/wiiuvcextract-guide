## How to extract ROMs from Wii U VC games

Before you begin, if you are using Windows, make sure that **File Name Extensions** is enabled in File Explorer, like in the image below.

<p align="center">
  <img src="https://i.imgur.com/Enayp9F.png" alt="File Explorer"/>
</p>

Also make sure that your USB storage device or SD card is formatted as FAT32.
If it is not, use one of these tools to do so:

Windows - [GUIFormat](http://ridgecrop.co.uk/index.htm?guiformat.htm)

Linux - [GParted](https://gparted.org/download.php)

MacOS - [Disk Utility](https://support.apple.com/guide/disk-utility/format-a-disk-for-windows-computers-dskutl1010)

MacOS Users: Always select "MS-DOS (FAT)", even if the card is larger than 32GB.

## NES/SNES/GBA/FDS/PCE/TurboGrafx-16

### What you need

* [wiiu-vc-extractor](https://github.com/wheatevo/wiiu-vc-extractor/releases/latest/) (download the respective .zip file for your operating system)

* An USB storage device or SD card with at least 300MB of free storage

* A Windows, Mac OS X or Linux computer with a USB port or SD card reader

#### Steps

**1.** Extract the contents of ``wiiu-vc-extractor-xxxxx-x64.zip`` to a folder on your computer.

**2.** Insert your USB storage device or SD card into your Wii U.

**3.** If prompted, **do not** format any USB devices through the Wii U.

**4.** Launch the internet browser on your console and open `dumplingapp.com`.

**5.** Tap "Launch dumpling".
    - If your console freezes for more than 10 seconds, hold down the Power button for 4 seconds and reboot.
    - Once rebooted, [reset the browser's save data](https://en-americas-support.nintendo.com/app/answers/detail/a_id/1507/~/how-to-delete-the-internet-browser-history) and try again.
    
**6.** Select "Dump Digital Games".

**7.** Select all the games you want to dump using the DPad/A button and then press Start.

**8.** Make sure the account is set accordingly, then select Start to begin dumping. (this could take a while)

**9.** Once finished, press start to exit Dumpling and insert your USB storage device or SD card into your computer.

**11.** Go into dumpling/games/[name of the game you dumped]/ on your USB storage device or SD card.  
● If your game is a NES/SNES/GBA/FDS/TurboGrafx-16 game, go into ``/code`` and copy the .rpx file into the same folder that you extracted wiiu-vc-extractor into.  
● If your game is a GBA game, go into ``/content`` and copy the .psb.m file and the .bin file into the same folder that you extracted wiiu-vc-extractor into.  
● If your game is a PCE game, go into ``/content`` and copy the .pkg file into the same folder that you extracted wiiu-vc-extractor into.

**12.** Run the following commands:

``cd [path to your wiiu-vc-extractor folder]``
``Linux and macOS only: chmod +x wiiuvcextractor``  
``wiiuvcextractor [dump file without the brackets]``

Congratulations, you now have your ROM! You can find the file in your wiiu-vc-extractor folder.

## Nintendo 64

### What you need

* An USB storage device or SD card with at least 300MB of free storage

* A computer with a USB port or SD card reader (an Android phone with an SD card slot also works great!)

#### Steps

**1.** Insert your USB storage device or SD card into your Wii U.

**2.** If prompted, **do not** format any USB devices through the Wii U.

**3.** Launch the internet browser on your console and open `dumplingapp.com`.

**4.** Tap "Launch dumpling".
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- If your console freezes for more than 10 seconds, hold down the Power button for 4 seconds and reboot.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Once rebooted, [reset the browser's save data](https://en-americas-support.nintendo.com/app/answers/detail/a_id/1507/~/how-to-delete-the-internet-browser-history) and try again.

**5.** Select "Dump Digital Games".

**6.** Select all the games you want to dump using the DPad/A button and then press Start.

**7.** Make sure the the account is set accordingly, then select Start to begin dumping. (this could take a while)

**8.** Once the dump has finished, press Start to exit Dumpling and insert your USB storage device or SD card into your computer/phone.

**9.** Go into dumpling/games/[name of the game you dumped]/content/rom/ on your USB storage device or SD card. There should be a single file in that folder. Rename its extension to ``.z64``.

**10.** Copy the file to a safe location on your device.

Congratulations, you now have your N64 ROM!

## Nintendo DS

### What you need

* An USB storage device or SD card with at least 300MB of free storage

* A computer with a USB port or SD card reader (an Android phone with an SD card slot also works great!)

#### Steps

**1.** Insert your USB storage device or SD card into your Wii U.

**2.** If prompted, **do not** format any USB devices through the Wii U.

**3.** Launch the internet browser on your console and open `dumplingapp.com`.

**4.** Tap "Launch dumpling".
    - If your console freezes for more than 10 seconds, hold down the Power button for 4 seconds and reboot.
    - Once rebooted, [reset the browser's save data](https://en-americas-support.nintendo.com/app/answers/detail/a_id/1507/~/how-to-delete-the-internet-browser-history) and try again.

**5.** Select "Dump Digital Games".

**6.** Select all the games you want to dump using the DPad/A button and then press Start.

**7.** Make sure the account is set accordingly, then select Start to begin dumping. (this could take a while)

**8.** Once the dump has finished, press Start to exit Dumpling and insert your USB storage device or SD card into your computer/phone.

**9.** Go into dumpling/games/[name of the game you dumped]/content/0010/ on your USB storage device or SD card. There should be a file called ``rom.zip`` and have a ``.nds/.srl`` file inside it. If it is an ``.srl`` file you can rename it to ``.nds`` and have it work that way.

**10.** Copy the file to a safe location on your device.

Congratulations, you now have your NDS ROM!

## Nintendo Wii

### What you need

* [nfs2iso2nfs](https://github.com/NicoAICP/UWUVCI-Tools/blob/master/nfs2iso2nfs.exe)

* [DumpsterU](https://github.com/GaryOderNichts/DumpsterU/releases/) (download the one for your OS)

* A ``otp.bin`` and ``seeprom.bin`` dump from your Wii U, if you dont have them follow this page: [Nand Dump](https://wiiu.hacks.guide/#/tiramisu/nand-backup)

* A Wii U formatted USB Drive with at least 4GB of free space (Copy the game(s) you want to extract to this before following the steps)

* A Windows or Ubuntu computer

* If you are using Windows, [.NET Framework](https://docs.microsoft.com/en-us/dotnet/framework/install/) version 4.5.2 or newer

* If you are using Ubuntu, [Wine](https://wiki.winehq.org/Download)
 
#### Steps

**1.** Insert the USB drive into your Computer. Do not format the drive if promted to.

**2.** Open up DumpsterU on your PC. Ubuntu users may have to open it through the terminal.

**3.** Select your USB drive and insert your ``otp.bin`` and ``seeprom.bin`` into DumpsterU and click ``Ok``.

**4.** Select the Game you want to extract and select a place to store it. (You have to do this step with every game you want to extract.)

**5.** Copy the ``nfs2iso2nfs.exe`` to the ``content`` folder of the dump.

**6.** Run ``nfs2iso2nfs.exe`` (You have to do this step with every game you want to extract.)

Windows:
```
cd [path to nfs2iso2nfs folder]
nfs2iso2nfs.exe -dec
```

Ubuntu:
```
cd [path to nfs2iso2nfs folder]
wine nfs2iso2nfs.exe -dec
```

Congratulations, you now have your Nintendo Wii ROM! 

## Issues

If you are having issues, read below. (If your issue is not present below, join the [Nintendo Homebrew Discord Server](https://discord.gg/C29hYvh) and ask for help in **#wiiu-assistance**)

### Nintendo Wii

**Q:** When running the exe I get "AES key missing". What do I do?   
**A.** You are missing htk.bin in the ``/code`` folder. Redump your game.

**Q.** When running the exe I get "Wii Common Key not found". What do I do?  
**A.** You are missing the wii common key in the dump. Get the wii common key from somewhere (your favorite search engine is your friend).

(will add more if more issues arise)

## Credits

* **lendun** for writing the wiiuvcextractor/N64/opening sections and figuring out how to select a default Github Pages theme

* **Lazr** for writing the DS/Wii/issues sections and helping with fact checking

* **Gary** and other Wii U helpers in the NH Discord server for helping with fact checking

* all the amazing developers who made the software used in this guide!
