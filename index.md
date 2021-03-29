## How to extract ROMs from Wii U VC games

Before you begin, if you are using Windows, make sure that **File Name Extensions** is enabled in File Explorer, like in the image below.

<p align="center">
  <img src="https://i.imgur.com/Enayp9F.png" alt="File Explorer"/>
</p>

Also make sure that your SD card is formatted as FAT32.
If it is not use one of these tools to do so:

Windows - [GUIFormat](http://ridgecrop.co.uk/index.htm?guiformat.htm)

Linux - [GParted](https://gparted.org/download.php)

MacOS - [Disk Utility](https://support.apple.com/guide/disk-utility/format-a-disk-for-windows-computers-dskutl1010)

MacOS Users: Always select "MS-DOS (FAT)", even if the card is larger than 32GB.

## NES/SNES/GBA/FDS/PCE/TurboGrafx-16

### What you need

* [wiiu-vc-extractor](https://github.com/wheatevo/wiiu-vc-extractor/releases/tag/2.0.0/) (download the respective .zip file for your operating system)

* [Dumpling](https://github.com/emiyl/dumpling/releases/tag/2.1.1) (download ``dumpling.zip``)

* An SD card with at least 300MB of free space

* A Windows, Mac OS X or Linux computer with an SD card reader

#### Steps

**1.** Insert your SD card into your computer.

**2.** Extract the contents of ``dumpling.zip`` to the root of your SD card.

**3.** Extract the contents of ``wiiu-vc-extractor-xxxxx-x64.zip`` to a folder on your computer.

**4.** Insert your SD card into your Wii U and power your Wii U on.

**5.** Launch The Homebrew Launcher using your preferred method.

**6.** Launch Dumpling.

**7.** Select "Dump Digital Games".

**8.** Select all the games you want to dump using the DPad/A button and then press Start.

**9.** Make sure the target destination is set to ``SD card`` and the account is set accordingly, then select Start to begin dumping. (this could take a while)

**10.** Once finished, press start to exit Dumpling and insert your SD card into your computer.

**11.** Go into dumpling/games/[name of the game you dumped]/ on your SD card.  
● If your game is a NES/SNES/GBA/FDS/TurboGrafx-16 go into ``/code`` and copy the .rpx into the same folder that you extracted wiiu-vc-extractor into.  
● If your game is a GBA game go into ``/content`` and copy the .psb.m file and the .bin file into the same folder that you extracted wiiu-vc-extractor into.  
● If your game is a PCE game go into ``/content`` and copy the .pkg file into the same folder that you extracted wiiu-vc-extractor into.

**12.** Run the following command:

``WiiuVcExtractor [dump file without the brackets]``  

Congratulations, you now have your ROM! You can find the file in your wiiu-vc-extractor folder.

## Nintendo 64

### What you need

* [Dumpling](https://github.com/emiyl/dumpling/releases/tag/2.1.1) (download ``dumpling.zip``)

* An SD card with at least 300MB of free storage

* A computer with an SD card reader (an Android phone with an SD card slot also works great!)

#### Steps

**1.** Extract the contents of ``dumpling.zip`` to the root of your SD card.

**2.** Insert your SD card into your Wii U and power your Wii U on.

**3.** Launch The Homebrew Launcher using your preferred method.

**4.** Launch Dumpling.

**5.** Select "Dump Digital Games".

**6.** Select all the games you want to dump using the DPad/A button and then press Start.

**7.** Make sure the target destination is set to ``SD card`` and the account is set accordingly, then select Start to begin dumping. (this could take a while)

**8.** Once the dump has finished, press Start to exit Dumpling and insert your SD card into your computer/phone.

**9.** Go into dumpling/games/[name of the game you dumped]/content/rom/ on your SD card. There should be a single file in that folder. Rename its extension to ``.z64``.

**10.** Copy the file to a safe location on your device.

Congratulations, you now have your N64 ROM!

## Nintendo DS

### What you need

* [Dumpling](https://github.com/emiyl/dumpling/releases/tag/2.1.1) (download ``dumpling.zip``)

* An SD card with at least 300MB of free storage

* A computer with an SD card reader (an Android phone with an SD card slot also works great!)

#### Steps

**1.** Extract the contents of ``dumpling.zip`` to the root of your sd card.

**2.** Insert your SD card into your Wii U and power your Wii U on.

**3.** Launch The Homebrew Launcher using your preferred method.

**4.** Launch Dumpling.

**5.** Select "Dump Digital Games".

**6.** Select all the games you want to dump using the DPad/A button and then press Start.

**7.** Make sure the target destination is set to ``SD card`` and the account is set accordingly, then select Start to begin dumping. (this could take a while)

**8.** Once the dump has finished, press Start to exit Dumpling and insert your SD card into your computer/phone.

**9.** Go into dumpling/games/[name of the game you dumped]/game/content/0010/ on your SD card. There should be a file called ``rom.zip`` and have a ``.nds/.srl`` file inside it. If it is an ``.srl`` file you can rename it to ``.nds`` and have it work that way.

**10.** Copy the file to a safe location on your device.

Congratulations, you now have your NDS ROM!

## Nintendo Wii

### What you need

* [nfs2iso2nfs](https://github.com/sabykos/nfs2iso2nfs/releases/tag/r2) (download ``nfs2iso2nfs.zip``)

* [Dumpling](https://github.com/emiyl/dumpling/releases/tag/2.1.1) (download ``dumpling.zip``)

* An SD card with at least 4GB of free space

* A Windows, Mac OS X (only pre-Catalina versions are supported) or Linux computer with an SD card reader

* If you are using Windows, [.NET Framework](https://docs.microsoft.com/en-us/dotnet/framework/install/) version 4.5.2 or newer

* If you are using Mac OS X or Linux, [Wine](https://wiki.winehq.org/Download) (You may need to install Wine-Mono, instructions can be found [here](https://github.com/Lazr1026/Guides-and-Shit-v2/wiki/Wine-Mono-Installation))
 
#### Steps

**1.** Extract the contents of ``dumpling.zip`` to the root of your sd card.

**2.** Insert your SD card into your Wii U and power your Wii U on.

**3.** Launch The Homebrew Launcher using your preferred method.

**4.** Launch Dumpling.

**5.** Select "Dump Digital Games".

**6.** Select all the games you want to dump using the DPad/A button and then press Start.

**7.** Make sure the target destination is set to ``SD card`` and the account is set accordingly, then select Start to begin dumping. (this could take a while)

**8.** Once the dump has finished, press Start to exit Dumpling and insert your SD card into your computer.

**9.** Go into dumpling/games/[name of the game you dumped]/content/ and extract the contents of ``nfs2iso2nfs.zip`` here.

**10.** If you are on Mac or Linux, launch Terminal.

**11.** If you are using Windows, run the exe ``nfs2iso2nfs.exe`` in the folder you extracted it to.

If you are using Mac or Linux, run the following commands:

```
cd [path to where you placed nfs2iso2nfs]

wine nfs2iso2nfs.exe -dec
```

Congratulations, you now have your ROM! You can find the file in the folder you ran the exe in.

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
