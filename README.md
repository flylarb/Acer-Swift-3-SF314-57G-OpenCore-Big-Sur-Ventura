# Acer-Swift-3-SF314-57G-OpenCore-Big-Sur-Ventura
<h2>Compatible with macOS Big Sur, Monterey and Ventura<h2>
<h3>What is this?
OpenCore is bootloader for booting macOS in your PC<h3>
<h3>Installing OpenCore<h3>
Download EFI.zip

Format USB Drive to FAT32 (At least 1GB for USB Drive)

If you didnt have USB Drive, You can partition internal drive and use new partition as OpenCore partition

Extract EFI.zip to your usb drive or partition (this can be in your internal drive)

Done

<h3>Installing macOS incase you didnt have USB Drive<h3>

Done the OpenCore install (in installing opencore that write upper here)

Get the macOS Recovery from macrecovery.py (get them from OpenCore Install Guide website in making the installer section)

Make new 20GB partition with exFAT for filesystem

Download Any Full macOS Installer (You can use Olarila for simple)

Open the macOS Installer you download using 7z and find Install macOS *Version you choose*.app (this locate in Applications folder)

Extract the Install macOS *version you choose*.app to 20gb partition you create eariler (not opencore partition)

Name the 20gb partiton as Installer

(read bios setup below before starting this process) Now boot to the opencore (it will name kingston rbusn8)

In OpenCore Boot Menu, Choose Recovery(*your version*).dmg

After you boot to setup, Open disk utility (you will need to hard clicking on trackpad or use mouse as normal click)

choose the partition you want to install macOS, Format them as APFS, incase it error to format as APFS format them as Mac OS Extended and convert them to APFS (it will locatw in menu bar, try checking all menu bar option for this)

exit disk utility

go to Utilities tab in menu bar and choose terminal

type this into terminal (case-sensitive)

"/Volumes/Installer/Install macOS Ventura.app/Contents/MacOS/InstallAssistant"

start installation and done!

this time after it reboot choose the boot disk to the macOS Installer option, keep repeating this until it change the drive name to the one you choose (like Untitled or Macintosh HD)

done

<h3>Spectifications<h3>

Intel Core i5 1035G1

Intel UHD Graphics 630 G1

Intel AX201

512GB Kingston M.2

HID Trackpad and Keyboard

8GB Ram

Nvidia GeForce MX250

<h3>What working<h3>
QE/CI of Intel UHD Graphics 630 G1

All USB ports

Display brightness

Wifi and Bluetooth

Internal speaker audio output

3.5mm Wired Headphone Input/Output

Keyboard backlit/backlight

Trackpad with all MacBook gesture

Front facing camera

Battery percentage

Handoff and import from iPhone (iPhone need to be on iOS 15 to make import from iPhone working)

Apple services (iMessages,FaceTime, iCloud)

<h3>Whats not working<h3>
Sleep and wake (fixing)

Internal microphone

HDMI (not tested)

Thunderbolt port (not tested)

AirPlay and AirDrop

Nvidia MX250 (Disable)

<h2>BIOS setup<h2>
Disable:

Secure Boot

Fast Boot
<h2>Enable:<h2>
F12 Boot menu
<h2>Change:<h2>
Sata mode to AHCI (Press ctrl+s at Main tab to show hidden option)

<h3>In order to use Windows without changing BIOS configuration, boot Windows using OpenCore and now it can be boot normally (no need to boot Windows using OpenCore anymore)<h3>
