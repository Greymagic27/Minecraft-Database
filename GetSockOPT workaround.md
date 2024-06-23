Step one - How do I know this is a firewall issue

On both your computers turn off the fire wall. Turn on the game on in both computers, setup a LAN game and make sure that the LAN game is visible to the other computer(if the LAN game is still not visible, this is not a firewall issue).
Turn the firewall back on!

https://support.microsoft.com/en-us/windows/turn-microsoft-defender-firewall-on-or-off-ec0844f7-aebd-0583-67fe-601ecf5d774f

​Step two - Allow Minecraft to pass through the firewall

- Open the firewall by typing windows defender firewall in start.
- Click on the Allow an app or feature through Windows Defender Firewall. This should give you a list of apps and features.
- Click the Change settings button to be able to add another app to the list.
- Click the Allow another app... button.
- In the new window click the Brows button.
- Navigate to your Minecraft installation folder:
  - Depending on the Minecraft launcher you use, the path you need to enter may vary.
    - For the legacy launcher (Grey creeper icon): C:\Program Files (x86)\Minecraft Launcher\runtime\java-runtime-delta\windows-x64\java-runtime-delta\bin
    - For the MS store launcher (Green creeper icon): C:\Users\User\AppData\Local\Packages\Microsoft.4297127D64EC6_8wekyb3d8bbwe\LocalCache\Local\runtime\java-runtime-delta\windows-x64\java-runtime-delta\bin

- Inside bin you should find a file exe called javaw.exe(or javaw if you don't show file extensions).
- Select that file and press the Open button and then press the Add button.

If there is no error you are done. Make sure to do this on both computers so both can create LAN servers.

If there is an error do the following steps.

1) The error should say something like: 'OpenJDK Platform binary' is already in the list of exceptions(if the name is different from OpenJDK Platform binary then use that name. Should be something that contains the word java).
2) Find OpenJDK Platform binary in the list of apps and delete it. This item should be pointing to a runtime that is not being used, hence the LAN not working. You can also use the details button to see where the item is pointing if you are nervous it does not belong to Minecraft.
3) Once you have deleted the item retry step one.
