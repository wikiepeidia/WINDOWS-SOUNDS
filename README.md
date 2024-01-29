# WINDOWS SOUNDS CHANGER REGEDIT TEMPLATE
This regedit file can quickly change all current Windows sounds to another Windows version's sound.

# Purpose:
If you are using Windows 10 but prefer Windows 11 sounds, or if you are on Windows 11 but prefer the sounds from Windows 7, this template can be useful for you.
However if you have like whatever custom sounds, renaming it is even more pain in the ### to just replace one by one.
Or you wanted how to make a custom scheme and transfer to another computer?

# How to:
I have prepared a Windows 10 sounds template for you. Use that template (windows 10's one) to perform.

For Windows 10 and earlier: Simply take ownership using `takeown /f c:\windows\media`, make a backup of that folder, then replace the Windows sounds with the ones you prefer. It's a simple process. But in case you can't find the sound on the internet and wanted to use mine, consider renaming it using whatever technique i posted below. You just need to replace WIN10 with nothing.
![POWERRENAME](https://github.com/wikiepeidia/WINDOWS-SOUNDS/blob/main/screenshot_1706513970.png)
For Windows 11, it seems that only some sounds such as notifications and the volume preview sound can be changed, while others does not.

Prepare the sounds of  Windows that you prefer.(INTERNET, or virtual machines,etc...)

don't  attempt to replace the filename directly, I recommend downloading PowerToys and using Power Rename. Windows 11 seems to consider the sound file's name, such as "Windows Notify," as the default, regardless of the actual sound it contains. Therefore, changing the name is important. Use the following settings in Power Rename to easily make these changes.
![POWERRENAME](https://github.com/wikiepeidia/WINDOWS-SOUNDS/blob/main/screenshot_1706512967.png)
REMEMBER: **CASE SENSITIVE!**
I do not recommend changing `$1` to anything else, but the suffix is your choice. This is because you also need to replace the name in the reg file. Open the reg file, use Ctrl H to find "WIN10," and change ALL instances to your preferred suffix. Also i recommend you also change your folder containing the sounds to whatever suffix you choose, just for convenience in replacing.

Finally: move that folder into `c:\windows\media` and run the reg file, enjoy.

For moving to other computer, open regedit: `Computer\HKEY_CURRENT_USER\AppEvents\Schemes` and export it out. Be sure that you check for the correct filenames and folder name to avoid errors.The picture below showing you must have folder named c:\windows\media\WIN8 and must have the file Speech MisrecognitionWIN8
![CHECK](https://github.com/wikiepeidia/WINDOWS-SOUNDS/blob/main/screenshot_1706514131.png) 
