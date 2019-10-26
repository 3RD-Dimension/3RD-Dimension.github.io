---
title: "The Settings Window"
permalink: /settings/
excerpt: "Information on the Settings Window"
sidebar:
  nav: "wiki"
toc: true
toc_label: "On this page"
---

## Connection Tab

![](/images/wiki/3rdd_settings_connection.png){: .align-center}
{:style="clear: center"}

The connection is where you can change settings relevent to the connection to your GRBL Controller.
* Serial Com Port.
* Baud Rate - From GRBL 1.1 Baud Rate is 115200.
* Reset GRBL when connecting - DTR signal is used to reset grbl when the connection is established.
* Controller Buffer - Arduino Uno controllers have a buffer of 127.  Arduino Mega controllers have a buffer of 255/256.
* Status Poll Interval (ms) - When to poll the controller for a status update.
* Log Traffic to file - Log any related message to a log file.  There is also another log file that any errors or info to do with the program is sent to a seperate file which is always enabled. This file is used to fix any bugs and may be asked for if an issue is opened.
* Ignore Additional Axes in Status Messages - Compatibility with custom GRBL versions which report 4+ axes in status reports.

## Viewport Tab

![](/images/wiki/3rdd_settings_viewport.png){: .align-center}
{:style="clear: center"}

This is where you can change various options of the job display.
* Preview Arc Segment Length (mm).
* Height Map Opacity (Currently not used and will be removed in future versions).
* Grid Thickness (default 0.1).
* Preview Toolpath.

## Probing Tab

![](/images/wiki/3rdd_settings_probing.png){: .align-center}
{:style="clear: center"}

Here you will find settings relevent to the probing button found on the [Probing / TLO Panel](https://3rd-dimension.github.io/probingpanel/).  When the probing button is clicked, the process will use these settings to probe and set Z0 for your tool automatically then raise.
* Probe Plunge Feed Rate (mm/min) - The rate that Z will lower until contact with your probe (Default 20 mm/min).
* Abort and Single on Probe Fail - If checked, an error will be displayed if probe cycle exceeded Max Probe Distance.
* Safe Retract Height (mm) - The amount Z will raise by after a successfull probing.
* Max Probe Distance (mm) - How far Z will lower to find yuor touch plate and if exceeds will abort.
* Probe Thickeness (mm) - Thickness of our probe/touch plate which will be used to set tool zero.

## GCode Tab

![](/images/wiki/3rdd_settings_gcode.png){: .align-center}
{:style="clear: center"}

This tab contains various options in relation to GCode, for the Sender and for the loaded file.
* Include Spindle 'S' Commands (Relevent to the loaded file).
* Include Dwell 'G4' Commands (Relevent to the loaded file).
* Include Program End (M2, M30) - These will be used to single the end of the job.
* Warning Window on File Load - If checked, information on what is being ignored when a file is loaded will be displayed.  **Note** any ingnored commands are only relevent to the displaying of the file, ingnored commands are still sent to the controller.
* FeedRate Inc/Dec - If checked feed rate will be increased or decreased by 10 each time (if using Hotkey).
* Spindle Inc/Dec - If checked Spindle will be increased or decreased by 10 each time (if using Hotkey).
* Zero All Command - Customise your Zero All Command sent to controller.
* Zero X Command - Customise your Zero X Command sent to controller.
* Zero Y Command - Customise your Zero Y Command sent to controller.
* Zero Z Command - Customise your Zero Z Command sent to controller.

## HotKey Tab 
**Added in Version 2.0.1.1**

![](/images/wiki/3rdd_settings_hotkey.png){: .align-center}
{:style="clear: center"}

The Hotkeys tab is where you can set Hotkeys for various commands.  Some hotkeys only work in certain states of the machine which will be noted.  **To set a key** Press the required key conbination into the fucntion you choose and it is set.  When you close the settings your hotkeys will be available.  To clear a hot key, double click with your mouse on the hoykey.

**Current Configurable Hotkeys**
* Jog X Axis + (Default: Right) - Only available if currently not sending a file and Jogging Keyboard Focused
* Jog X Axis - (Default: Left) - Only available if currently not sending a file and Jogging Keyboard Focused
* Jog Y Axis + (Default: Up) - Only available if currently not sending a file and Jogging Keyboard Focused
* Jog Y Axis - (Default: Down) - Only available if currently not sending a file and Jogging Keyboard Focused
* Jog Z Axis + (Default: Numpad 9) - Only available if currently not sending a file and Jogging Keyboard Focused
* Jog Z Axis - (Default: Numbpad 3) - Only available if currently not sending a file and Jogging Keyboard Focused
* Emergency (Default: Escape) - Available always
* Cycle Start - Starts sending file if not currently being sent
* File Hold / Jog Cancel - Cancels jogging (if jogging) or Holds if a file is currently being sent
* Return to Origin (Zero of X, Y, Z) - Only available if machine is idle
* Spindle Increase - Only available if currently running a file
* Spindle Decrease - Only available if currenltly running a file
* Feed Rate Increase - Only available if machine is sending
* Feed Rate Decrease - Only available if machine is sending
* Jog Rate Increase - Only available if machine is idle or jogging
* Jog Rate Decrease - Only available if machine is idle or jogging
* ReDo/Reload Last File - Only available if machine is idle
* Spindle On/Off - Firmware takes care of when it can be used
* Coolant On/Off - Firmware takes care of when it can be used
* Mist On/Off - Firmware takes care of when it can be used