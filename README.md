cam4-anonymous
====================
cam4-anonymous lets you follow and archive your selected models' shows on www.cam4.com
You don't need to be registered cam4 user for recording models with this cam4-anonymous script.

Requirements
============
1. Download here [Python 2.7.13](https://www.python.org/ftp/python/2.7.13/python-2.7.13.msi) instalation. Those who need to install python should watch this [video](https://www.youtube.com/watch?v=QYUBz4mrnFU)
2. Download here [RTMPDump(ksv)](https://github.com/K-S-V/Scripts/releases) used for recording the streams.
3. Download here [ffmpeg and ffplay](https://ffmpeg.zeranoe.com/builds/) who must be somewere in the path, default location is 'C:/Windows'
4. Download here [youtube-dl](https://github.com/rg3/youtube-dl) who must be somewere in the path, default location is 'C:/Windows'

Setup
=====
1. Download entire code as ZIP from Github, extract the C4 folder to C:\cmd\ (for minimal edits in configs).
2. Open "Requirements" folder, install Python 2.7.13 (python-2.7.18.exe) and Python 3.9.0 (python-3.9.0-amd64.exe) in successive order.
3. Once Python is installed, go to root folder, C:\cmd\C4 , open cmd or powershell here and enter 'pip install -r Requirements.txt' and then 'pip install -r Requirements3.txt'
Note: Step 4, 5, 6 and 7 are optional as both, Streamlink and Livestreamer will automatically install using pip, however they might not be in the default locations that are set in the C4.bat and C43.bat, and hence you can either choose to edit the files to set the right location, or else, use this to make sure it gets installed in specified paths as per code, so no errors occur.
4. Install Chocolatey in Powershell using command "Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))"
5. In Powershell enter following command to install Streamlink "choco install streamlink --version=1.7.0"
6. In Powershell enter following command to install Livestreamer "choco install livestreamer"
7. If you are semi-advanced user, and know how to play with the code, you can open C4.bat and C43.bat and config.ini and config3.ini and alter values as per the paths on your system, you could face some errors, which will fix as you go on fixing the paths.
8. Add Path to Environment Variables. You can search for Path in Start Menu (windows 10/11) and an option "Edit the System Environment Variables" will show up, click on that, then the "Environment Variables" option on there.
9. There will be Variable named "Path" double click, select "New" add "C:\cmd\C4\Requirements\ffmpeg-20200831-4a11a6f-win64-static\bin" (without " "), click "New" again, add "C:\cmd\C4\Requirements\trmpdump", click "New" again, add "C:\cmd\C4\Requirements".
10. This has added the tools required to dump the stream into a file with different options, like Streamlink, Livestreamer, YouTube-DL, FFMPEG.
11. Then, proceed to the "C4_Wanted" file, add the models you wish to add to your list for recording, go to stream/profile, copy the username after the URL, (For Example: www.cam4.com/hazelmoore | In this, the thing you need to copy is hazelmoore) and paste it in the file, one name in each line, remember to put an empty line after the last model name is entered (code bug)
12. Open C4.bat (preferred) or C43.bat, select your preferred options for stream recording (personal preference is 2->0->select model as per your list->2 as Streamlink gives mp4 output and is stabler)

Running & Output
================
It's best to use 'Command Promt' first to install `Requirements.txt`. You can also install the modules individually with the command 'pip install SomePackage==1.0.4 # specific version'
For use these scripts it would be good to make a shortcut for `c4.bat` and put it in the task bar for easier startup. 
All scripts using the same text file where is stored models for recordings, default is `C:\-c4-py\C4_Model.txt`. 
However, if you want to record a certain model permanently (24/7), then you need to use `c4.bat`, options numbers 2 to 5 for start rtmpdump, youtube-dl, ffmpeg or streamlink.
Default script is 'c4a.py' letter 'a' in the name means 'ALL' for 'all mode' record and play with hidden script traffic. 
Script 'c4aw.py' letter 'w' in the name means 'window' allow you to see what is actually happening in a separate window and make it easier to stop recording.
If you want to record more models at the same time then you need to start another copy of `c4.bat`. 
All scripts have the ability to display some basic data about the models (Age, Location, Relationship Status and Occupation - Job).
Break recording is with with Ctrl-C or by clicking 'x' at the top right corner of the script window If Ctrl-C does not react.

screenshot0:

![alt screenshot](./screenshot0.jpg)

screenshot1:

![alt screenshot](./screenshot1.jpg)

screenshot2:

![alt screenshot](./screenshot2.jpg)
