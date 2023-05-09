# YuzuManyPlayersTool
This is a simple script, a "Flow" written with Microsoft's Power Automate. So you need Windows to use this.
It lets more than 1 user to be able to play a yuzu game with different saves while sharing other settings.
Just prompts asking if you're Player1 or Player2, then does its thing with save files and finally opens yuzu.

You will spend like 10 minutes setting this up and then it will save you time whenever a different user wants to play.

# Disclaimer
I am not responsible for any damage or loss of your files. If you're trying this you should make backups of every save file that will be involved in this, and do not start playing until you check that everything is working as expected. 

# Setup
In order to use this script you will need a free or premium MS account inside Power Automate. 
Premium users (there's a 90 day free trial without credit card) can send the flow to their desktops as a shortcut.

First of all, download the "oldsaves" folder and place it anywhere you like. After doing that, open Power Automate and create a new flow, call it what you like. Then copy the contents of "PasteInsidePowerAutomateFlow" to the Main flux (CTRL-V). Now for the script to work, you should change all needed Paths to your needs. It should be pretty much straight-forward.

When everything is well set up, copy the save folders (they are called the same as GAMECODE and contain a bunch of folders usually) to oldsaves/(each player), so there is a save file for each player and the save file inside yuzu. You can delete the "placeholder" files. Check that it works and save it, and then to use it just press play inside Power Automate or (if you have Power Automate premium) right-click, and then press Shortcut To Desktop. Note that, if you don't want Power Automate's window to open everytime you play the game, you should uncheck the "Show confirmation dialog when invoking a flux externally" option in settings. You could also deactivate windows notifications. That way you won't even notice that Power Automate is working.

If you don't know what do you need to change in the Paths, go to Yuzu, right-click your game and press Open Save Data Location. The name to that folder is GAMECODE. The folder over that, that has a longer name is YOURCODE. Before \\user\\nand you should paste your actual route to that folder (it could be something like "D:\\Games\\Yuzu\\user\\nand..."). And before \\oldsaves paste the route where you downloaded the folder.
