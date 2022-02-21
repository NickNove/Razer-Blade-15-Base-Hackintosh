# Razer-Blade-15-Base-Hackintosh
A dump of my EFI as well as basic info for getting started.

NOTE: !!!I AM BY NO MEANS AN EXPERT AT HACKINTOSHING AND AM NOT OFFERING ADVICE, INSTRUCTIONS, OR GUIDANCE IN THE PROCESS OF RUNNING MACOS ON NONAPPLE DEVICES. ANYTHING YOU DO YOU ASSUME LIABILITY FOR AND I AM NOT RESPONSIBLE FOR ANYTHING THAT HAPPENS TO YOUR DEVICE!!!

This is a paste of my EFI folder I use for my 2018 Razer Blade 15 Base Model laptop (Model#: RZ09-03006E92) to run MacOS Monterey 12.2.1. I cannot guarantee that it will work for you even on an identical system and would not recommend using these files as anything other as a starting point to create your own.

Some resources I found helpful when creating my Hackintosh were:
https://github.com/DocSystem/razerbladehackintosh
https://www.youtube.com/watch?v=oxQU3IrGqCM
https://dortania.github.io/OpenCore-Install-Guide/
https://mackie100projects.altervista.org/download-opencore-configurator/
and many other forums and posts.

PLEASE NOTE THE FOLLOWING:
You will need to download a fresh copy of OpenCore 0.7.8 and move the EFI>OC>Resources directory to this EFI>OC directory as it was too many files for me to easily upload to this repository (over 400).
Please note I have cleared the following values from the config.plist file and you will need to populate them with uniquely generated ones yourself. (This is easily accomplished following any number of guides online):

DataHub
+SystemSerialNumber
+SystemUUID

Generic
+SystemUUID
+SystemSerialNumber
+MLB
+ROM

PlatformNVRAM
+BID
+FirmwareFeatures
+FirmwareFeaturesMask
+MLB
+ROM
+SystemSerialNumber
+SystemUUID

SMBIOS
+BoardSerialNumber
+ChassisSerialNumber
+SystemSerialNumbr
+SystemUUID
