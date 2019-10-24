---
title: "The Machine Panel"
permalink: /machinepanel/
excerpt: "Information on the Machine Panel"
sidebar:
  nav: "wiki"
toc: true
toc_label: "On this page"
---

![](/images/wiki/3rddgcs_machine_main.png){: .align-center}
{:style="clear: center"}
The machine panel is the main panel that you use to connect to your machine, change settings, view GRBL settings and G5x work offsets.

The connect/disconnect button is self-explanatory - use this to connect or disconnect from your machine.  The settings button allows you to change different settings.

The bar below the connect and settings button is the current buffer status of your GRBL controller.

Below the buffer bar is a drop down to select your desired work offset - the default (and what is selected on program start up and controller connect) is G54.  You can also select if needed G55-G59 work offsets manually.  Note that if there is a G5x in your code - that will override what you have selected.

Also on this panel is the Home button - click this to home the machine.

## Work Offsets

![](/images/wiki/3rddgcs_machine_offsets.png){: .align-center}
{:style="clear: center"}

Clicking on the Work Offsets button will display the above screen.  This is where you can Set, Change or reset each of the G5x work offsets for the machine.  **Note** *The G5x workoffsets are stored in your GRBL controller (persistant) until you reset them.

* **Setting Work Offsets**

    * To set a work offset for all axis to the current machine location - Click on the desired G5x button on the left.  This will set and save X, Y and Z offset values.
    * To set only one of the axis - change the desired G5x axis, and then double-click in the field - this will save only that axis and value without desturbing the others.
    * To reset the desired G5x to Zero - click on the Reset button on the right for that work G5x offset.

## GRBL Settings

![](/images/wiki/3rddgcs_grblSettings.png){: .align-center}
{:style="clear: center"}

At the top of this window the current version of your GRBL controller is displayed as well as any options associated with it.

Below this is all the current settings on the controller which you can change and then save by clicking on "Apply" - the new settings will be saved to the Eeprom.  If you dont know what each setting does, a short description is also shown.

There is also an "Export" button where you can export the currently displayed settings to a text file in an easy-to-read format.  Very usefull for backing up the settings for future use or testing.

Here is an example of the exported file
![](/images/wiki/3rddgcs_machine_grbl_export_sample.png){: .align-center}
{:style="clear: center"}