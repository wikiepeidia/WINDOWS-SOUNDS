# WINDOWS-SOUNDS
This regedit file can quickly change all Windows sounds.

# Purpose:
If you are using Windows 10 but prefer Windows 11 sounds, or if you are on Windows 11 but prefer the sounds from Windows 7, this template can be useful for you.

# How to:
I have prepared a Windows 10 sounds template for you. If you prefer older sounds such as those from Windows 8 or 7, you can use Chat GPT to assist with the change.

For Windows 10 and earlier: Simply take ownership using `takeown /f c:\windows\media`, make a backup of that folder, then replace the Windows sounds with the ones you prefer. It's a simple process.

For Windows 11, it seems that only some sounds such as notifications and the volume preview sound can be changed, while others does not.

Prepare the sounds in Windows that you prefer.

don't  attempt to replace the filename directly, I recommend downloading PowerToys and using Power Rename. Windows 11 seems to consider the sound file's name, such as "Windows Notify," as the default, regardless of the actual sound it contains. Therefore, changing the name is important. Use the following settings in Power Rename to easily make these changes.

I do not recommend changing `$1` to anything else, but the suffix is your choice. This is because you also need to replace the name in the reg file. Open the reg file, use Ctrl H to find "WIN10," and change ALL instances to your preferred suffix. Also i recommend you also change your folder containing the sounds to whatever suffix you choose, just for convenience in replacing.

Finally: move that folder into `c:\windows\media` and run the reg file, enjoy.
