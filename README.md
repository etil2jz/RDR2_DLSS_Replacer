# RDR2 DLSS Replacer
Rockstar Launcher replaces DLSS file with their own version every time you start Red Dead Redemption 2. This app bypasses this problem, so you can use your preferred DLSS version easily.

Run it before launching RDR2, it will replace DLSS with your preferred version, and when you exit RDR2 it will restore original DLSS file so that Rockstar Launcher does not update the game every time you launch or exit game.

## How to use
1. Download from: https://github.com/Bullz3y3/RDR2_DLSS_Replacer/releases/latest
2. Extract it.
3. Run `RDR2_DLSS_Replacer.exe`
   - It needs Administrator Privileges to replace `nvngx_dlss.dll` in RDR2 directory.
   - It requires .NET Framework 4.7.2+ installed. [Download from Microsoft.](https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net472-offline-installer)
   - It will download DLSS/nvngx_dlss_3.7.10.dll automatically when you run it for the first time. 
     - (Optional) If you want to use your own preferred DLSS file then paste it in the folder of RDR2_DLSS_Replacer.exe and name it as nvngx_dlss.dll
4. Start Red Dead Redemption 2 game.

`RDR2_DLSS_Replacer.exe` can be kept open for as long as you want, it does not exit with the game, so you can launch or exit the game multiple times and it will keep processing.

_(Optional)_ **Auto launch RDR2** when you start this app.
   - Open `rdr2_location_for_auto_start.txt`
   - Provide absolute location to RDR2.exe at end of file.

## How it works
It monitors `RDR2.exe` process in task manager an as soon as it finds the process, it immediately replaces the game's DLSS in the game's location and creates backup of original DLSS file. Similarly, when the `RDR.exe` process exits it reverts back DLSS. Your game location can be anywhere, it will be detected automatically by this app.