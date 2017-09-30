---
layout: post
title: The FSR Joystick
- joystick_mouthpiece_path: /_resources/images/joystick_mouthpiece.jpg
  title: Joystick with mouthpiece
- fsr_path: /_resources/images/fsr.jpg
  title: FSR
- frontchamber_path: /_resources/images/frontchamber.jpg
  title: pressure sensor
---

Remember how after we had scrapped the PS2 joystick, we had narrowed our joystick options down to two? Well, we’ve chosen the one to move forward with.

<img src="https://raw.githubusercontent.com/makersmakingchange/blog/gh-pages/_resources/images/joystick_mouthpiece.jpg" title="Joystick with mouthpiece"/>

<em><strong>Above: A picture of the joystick module with the mouthpiece attached.</strong></em>

<em><strong>Below: The bottom half of the joystick with the Force Sensitive Resistors (FSRs).</strong></em>

<img src="https://raw.githubusercontent.com/makersmakingchange/blog/gh-pages/_resources/images/fsr.jpg" title="FSR"/>

We’ve decided to go with the Force Sensitive Resistor (FSR)-based joystick, which rather than using a manufactured joystick (like a medical one, or a PS2 or PSP one), relies on four FSRs to control movement.

We had also contemplated using the PSP joystick. However, its design caused several problems. One such problem was that it was translational, rather than rotational as most joysticks are. If you think of a typical joystick — think of the PS2 joystick, if you play video games — the joystick can be twirled all-around, not just on a linear basis like the PSP one. For one, this would extend the length of the joystick apparatus, and in addition, caused the joystick to get jammed.

The FSRs, on the other hand, are thin. They are relatively inexpensive, at about $10 per resistor (you need four). When all is said and done, this “homemade” joystick will probably cost between $40 and $50. While it is not as cheap as the $2 PS2 joysticks we were initially contemplating, these are much more accurate, much more reliable, and much more stable. The quality is more akin to $300 medical joysticks — the FSR joystick is the perfect blend of cost-effectiveness and quality. The FSR joystick design is also significantly shorter than our previous design, taking more than a full inch off the length of the device. 

However, there are still some bugs to be worked out, as we work to freeze the design.

<img src="https://raw.githubusercontent.com/makersmakingchange/blog/gh-pages/_resources/images/frontchamber.jpg" title="Front chamber"/>

<em><strong>The redesigned front chamber, made to limit joystick movement.</strong></em>

One of the problems with the FSR joystick is that, on some of our test builds, it has a tendency to drift when you push it too far in one direction — the cursor will continue to move slowly after you let go of the joystick. However, this only seems to be an issue when you take the joystick as far as it can go — to its max. We’ve made a redesigned front chamber (pictured above), which is designed specifically to limit such movement. We are also working on a software calibration solution.

As well, the joystick currently makes too much noise. When moving it, you can hear clicking sounds and squeaking — which would be quite annoying to the user. We’re working on a few solutions to this. We are currently experimenting with a number of different types of springs. Another solution is filing down the rubber feet (the white tube-like structures), which have a tendency of sticking to the FSRs.

We’ve got a lot of work to do over the next three weeks as we have a number of upcoming events and people eager to receive a LipSync. Over that time, we also need to do some user testing and get some feedback so that we can finalize the design. It’s going to be busy, but we’re looking forward to the next stage.

