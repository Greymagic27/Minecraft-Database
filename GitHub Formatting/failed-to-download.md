## **Potential Workaround (Windows 10/11):**

Things to try first:
 * Delete .minecraft folder: https://minecrafthopper.net/help/finding-minecraft-data-folder/
 * Change DNS: https://1.1.1.1/dns/#setup-instructions

### <u> For Missing Java: </u>
<ul>
 <li> <strong>1.18-1.19:</strong> Download Java 17: https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_windows_hotspot_17.0.6_10.msi, run that, find the javaw.exe file in C:\Program Files\Eclipse Adoptium\jdk-17.0.6.10-hotspot\bin. Click on Installations in the Minecraft launcher, click Edit Installation on your installation, click more options, and set the Java Runtime to be directed to the javaw.exe. </li>
 <li> <strong>1.17:</strong> Download Java 11: https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.18_10.msi, run that, find the javaw.exe file in C:\Program Files\Eclipse Adoptium\jdk-11.0.18.10-hotspot\bin. Click on Installations in the Minecraft launcher, click Edit Installation on your installation, click more options, and set the Java Runtime to be directed to the javaw.exe. </li>
 <li> <strong>1.8.9-1.16.5:</strong> Download Java 8: https://www.java.com/en/download/, run that, find the javaw.exe file in C:\Program Files\Java\jre1.8.0_351\bin. Click on Installations in the Minecraft launcher, click Edit Installation on your installation, click more options, and set the Java Runtime to be directed to the javaw.exe.
</ul>

### <u> For Missing Files: </u>

This is a little difficult to do, so feel free to ask questions.

First, we need to get the file on your system. To do this, open Command Prompt.

To get the URL of the missing file, we need to look at the error generated. After the error says "URL:", copy the entire path. Ex: https://resources.download.minecraft.net/aa/aa1d3aace1c481ac32d5827fba287294b6bc99fb.

Now, run this command in your Command Prompt replacing "\<url>" with the URL you copied above.
<BR>

`cd Downloads && curl -O <url>`

<BR>

Notice how in that URL it says minecraft.net/**xx**/, those two bolded letters or numbers signify the name of the folder this file needs to go in. Run Windows + R and type in `%AppData%`. Press enter and navigate to the .minecraft folder. Locate the assets/objects folder. In here, create a folder with the same two letters or numbers that your URL says. If it already exists, navigate to it.

Find your Downloads folder, and drag and drop the file we just downloaded into the folder we just navigated to.

Wow! You did it! Now, do that for every file it throws an error for. I know, it's painful.

## **Potential Workaround (Mac OS):**

Things to try first:
 * Delete .minecraft folder: https://minecrafthopper.net/help/finding-minecraft-data-folder/
 * Change DNS: https://1.1.1.1/dns/#setup-instructions
 
### <u> For Missing Java: </u>

<ul>
 <li> <strong>1.18-1.19:</strong> Download Java 17: https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_mac_hotspot_17.0.6_10.pkg, run that, and follow the instructions.
 <li> <strong>1.17:</strong> Download Java 11: https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_mac_hotspot_11.0.18_10.pkg, run that, and follow the instructions.
 <li> <strong>1.8.9-1.16.5:</strong> Download Java 8: https://www.java.com/en/download/, run that, and follow the instructions.
</ul>

After installing Java, we need to set make Minecraft use it. Click on the Installations tab of the launcher and click Edit Installation next to your version. Click More Options, and click to change the Java Runtime. Once you're in the Finder window it opens, you need to run Cmd + Shift + G. Type into that little box, "~/Library". Locate the Java folder (or Eclipse Temerium), select the version as downloaded above, locate the bin folder, and select the javaw file.

### <u> For Missing Files: </u>
This is a little difficult to do, so feel free to ask questions.

First, we need to get the file on your system. To do this, open Terminal.

To get the URL of the missing file, we need to look at the error generated. After the error says "URL:", copy the entire path. Ex: https://resources.download.minecraft.net/aa/aa1d3aace1c481ac32d5827fba287294b6bc99fb.

Now, run this command in your Terminal replacing "\<url>" with the URL you copied above.
<BR>

`cd Downloads && curl -O <url>`

<BR>

Notice how in that URL it says minecraft.net/**xx**/, those two bolded letters or numbers signify the name of the folder this file needs to go in. Open finder, and run Cmd + Shift + G. Type in that box "~/Library" and click enter. Locate the Application Support folder, and enter it. The .minecraft folder will be found in here, open it. Locate the assets/objects folder. In here, create a folder with the same two letters or numbers that your URL says. If it already exists, navigate to it.

Find your Downloads folder, and drag and drop the file we just downloaded into the folder we just navigated to.
