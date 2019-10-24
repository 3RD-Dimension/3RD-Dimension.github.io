---
title: "The Probing Panel"
permalink: /probingpanel/
excerpt: "Information on the Probing Panel"
sidebar:
  nav: "wiki"
---

![](/images/wiki/3rddgcs_probing_tlo.png){: .align-center}
{:style="clear: center"}
The probing panel is pretty basic in its curernt form (Will be extended in future) and currently can be used to set offsets for additional tools that are used in the job.

**Probing initial tool**

For normal probing and setting Zero for that tool (and all settings in the probing settings are entered) - clicking on the button will start the probing command.

To do probing, move your Z axis over your touch-plate and then click on the button.  Z axis will slowly lower until it touches the touch plate, it will then set Z to Zero and then raise by a determined amount (in the settings window).

**Probing additional tools**
1. Load initial tool.
1. Move the machine to the tool length sensor (touch-off plate perhaps).
1. Touch of Z with the relevent G38 command.
1. Click on "Save Pos" - this will save the position of the last probe cycle as the position.
1. Continue with your job until the next tool change is required.
1. Change to the next tool, move to the tool length sensor or touch-off plate and touch off again (new tool needs to be roughly at same height of the initial tool).
1. Now, click on "Apply TLO" and it will compute the new offset for the new tool.
1. Continue with the next operation.