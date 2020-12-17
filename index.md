### How to extract ROMs from Wii U VC games

Before you begin, if you are using Windows, make sure that **File Name Extensions** is enabled in File Explorer, like in the image below.

<p align="center">
  <img src="https://i.imgur.com/Enayp9F.png" alt="File Explorer"/>
</p>

Also make sure that your SD card is formatted as FAT32.

## NES/SNES/GBA/FDS/PCE/TurboGrafx-16

### What you need

* [wiiu-vc-extractor](https://github.com/wheatevo/wiiu-vc-extractor/releases/tag/0.9.0) (``download wiiu-vc-extractor-0.9.0.zip``)

* [Dumpling](https://github.com/emiyl/dumpling/releases/tag/2.1.1) (download ``dumpling.zip``)

* An SD card with at least 300MB of free space

* A Windows, Mac or Linux computer with an SD card reader

* If you are using Windows, [.NET Framework](https://docs.microsoft.com/en-us/dotnet/framework/install/) version 4.5.2 or newer

* If you are using Mac or Linux, [Mono](http://www.mono-project.com/docs/getting-started/install/)

#### Steps

**1.** Insert your SD card into your computer.

**2.** Extract the contents of ``dumpling.zip`` to the root of your SD card.

**3.** Extract the contents of ``wiiu-vc-extractor-0.9.0.zip`` to a folder on your computer.

**4.** Insert your SD card into your Wii U and power your Wii U on.

**5.** Launch The Homebrew Launcher using your preferred method.

**6.** Launch Dumpling.

**7.** Select "Dump Digital Games".

**8.** Select all the games you want to dump using the DPad/A button and then press Start.

**9.** Make sure the target destination is set to ``SD card`` and the account is set accordingly, then select Start to begin dumping. (this could take a while)

**10.** Once finished, press start to exit Dumpling and insert your SD card into your computer.

**11.** Go into dumpling/games/[name of the game you dumped]/code/ on your SD card and copy the file with the extension ``.rpx`` (the file extension will be ``.psb.m`` if you are extracting a GBA game, ``.pkg`` if you are extracting a PCE game) into the same folder that you extracted wiiu-vc-extractor into.

**12.** Launch Command Prompt if you are on Windows. If you are on Mac or Linux, launch Terminal.

**13.** If you are using Windows, run the following commands:

```
cd [path to your wiiu-vc-extractor folder without the brackets]

WiiuVcExtractor [dump file without the brackets]
```

If you are using Mac or Linux, run the following commands:

```
cd [path to your wiiu-vc-extractor folder without the brackets]

mono WiiuVcExtractor [dump file without the brackets]
```

Congratulations, you now have your ROM! You can find the file in your wiiu-vc-extractor folder.

## Nintendo 64

### What you need

* [Dumpling](https://github.com/emiyl/dumpling/releases/tag/2.1.1) (download ``dumpling.zip``)

* An SD card with at least 300MB of free storage

* A computer with an SD card reader (an Android phone with an SD card slot also works great!)

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

