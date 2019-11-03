---
permalink: /quickstart/
title: "Quick Start Guide"
author_profile: true
toc: true
toc_label: "On this page"
---

Welcome to the Quickstart guide.  Follow this guide to get up and running as easily and quickly as possible.

## Requirments
There are only a couple of requirments needed to run 3RDD GCode Sender
* Microsoft .NET Framework 4.6 [Download .NET 4.6](https://dotnet.microsoft.com/download/dotnet-framework/net462)
* Microsoft Windows 10 32/64.  Windows 7 has not been tested but might work.  Windows XP Not Supported, Linux not supported (as WPF framework is not supported).
* GRBL 1.1x [Uno](https://github.com/gnea/grbl) or [Mega](https://github.com/gnea/grbl-Mega/) (<= 0.9 will not work and not supported)

3RDD GCode Sender is compiled using Visual Studio 2019.

## Step 1 - Download latest version
1. Go to our Github page and [download the latest version](https://github.com/3RD-Dimension/3RDD-GCode-Sender-Issues/releases).
1. Unzip/Extract the zip file to a folder of your choosing.

## Step 2 - Start the program
When you have extracted to a folder, locate the directory and double-click on **3RDD GCode Sender.exe** and you will be presented with the following.
![Step 2](/images/quickstart/step2.png)

## Step 3 - Configure to connect to GRBL
1. Locate the **Machine** panel on the top-right of the window and click on it - it will expand revealing more options.
1. Click on **Settings**.
1. Select your serial port that your controller is connected to.
1. Change the BaudRate if its different - GRBL is usually 115200.
1. If you want to soft-reset the controller when connecting, tick _Reset grbl when connecting_.  The Mega version of GRBL sometimes has an issue if this is checked - if you find when connecting you do not see the initialization from the controller and you have this checked, uncheck it and try again.  You can then Soft Reset manualy if needed.
1. Change Controller Buffer - If using GRBL on Uno buffer is 127.  GRBL on Mega is 255.
1. The last 3 options (Status Poll, Log Traffic to File, Ignore Additional Axis) are up to you.

## Step 4 - Connect to your Controller
Once you have made the required changes above, you can now connect to your controller.  To do this - in the Machine panel click on **Connect** and you should see the initialization from your controller at the bottom right.
![Step 2](/images/quickstart/step4.png)

From this point on, all controller and machine options will now become available - you can now jog your machine, load a GCode file, run a file as well as change GRBL controller settings straight from the program.

Any issues [please let us know](https://github.com/3RD-Dimension/3RDD-GCode-Sender-Issues/issues)