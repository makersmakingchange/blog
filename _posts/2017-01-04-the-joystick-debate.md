---
layout: post
title: The Joystick Debate
- ps2_joystick_path: /_resources/images/PS2_joystick.jpg
  title: PS2 joystick
- psp_joystick_path: /_resources/images/PSP_joystick.jpg
  title: PSP joystick
- pressure_sensor_path: /_resources/images/pressure_sensor.jpg
  title: pressure sensor
---

In the last days of 2016, the [LipSync](http://www.neilsquire.ca/research-development/projects-activities/lipsync/) team is working hard to “freeze” the design ahead of the [Access Makeathon](https://www.eventbrite.com/e/access-makeathon-vancouver-2016-tickets-3473530423) on January 27th.

There’s one thing, though, that we’re still trying to nail down — the joystick.

<img src="https://raw.githubusercontent.com/makersmakingchange/blog/gh-pages/_resources/images/PS2_joystick.jpg" title="PS2 joystick"/> 


<em><strong>The original joystick we intended to use — the PS2 (PlayStation 2) thumb joystick (two of them side-by-side in the picture — one with thumb-pad, one without).</strong></em>

Back in July, [we were planning](http://www.neilsquire.ca/latest-news/technology-news/lipsync-update-joystick/) on using the [PS2 (PlayStation 2)](https://en.wikipedia.org/wiki/PlayStation_2) thumb joystick. Before testing, it had seemed like a great option, as they were adaptable, durable, and cheap (you could find one for $2).

Our user-testing showed that the range of motion needed to move the joystick was too much for people with neck injuries — the PS2 joystick wasn’t sensitive enough. While previously developed technologies like the [Jouse](http://www.neilsquire.ca/research-development/projects-activities/jouse/) were sensitive enough to require little movement, ours required a lot of head movement.

While we did try some solutions to increase the sensitivity, it became clear that the PS2 joystick just wasn’t going to work. While it was an affordable option, pain is an unacceptable cost for the user.

So we’ve come up with some other options.

<img src="https://raw.githubusercontent.com/makersmakingchange/blog/gh-pages/_resources/images/PSP_joystick.jpg" title="PSP joystick"/> 

<em><strong>A joystick prototype using a PSP (PlayStation Portable) joystick. In this picture, the mouthpiece is attached.</strong></em>

The first of these options doesn’t stray far from the original idea of repurposing PlayStation joysticks — this time we’re using a [PSP (PlayStation Portable)](https://en.wikipedia.org/wiki/PlayStation_Portable) joystick.

While the PS2 joystick had too much slop, the PSP joystick is much more sensitive. The pressure is controlled by springs attached to the screws. In that area, (where you see pink in the photo — it’s hard to see), there’s a 3D printed ball placed in there that makes the motion more smooth, more finite than the PSP itself.

However, this prototype is not without problems. As you can see from the picture, this does make the LipSync a lot bigger — a bigger head chamber would be needed, which is not an ideal solution. As well, the ball which makes motion a lot smoother does create some difficulties. It’s hard to get the ball smooth. Though we used wax to help the end product, every printer is different and it can be different printing round shapes that are smooth.

<img src="https://raw.githubusercontent.com/makersmakingchange/blog/gh-pages/_resources/images/pressure_sensor.jpg" title="Pressure sensor"/>

<em><strong>This prototype doesn’t actually use a joystick, but instead, uses pressure sensors. The mouthpiece is not pictured here.</strong></em>

Our other idea takes things in a bit of a different direction. The other joystick prototype doesn’t even use a joystick. Instead, it controls movement through four pressure sensors — four sensitive resistors (seen in the picture attached to wires).

This is closer to the system that the [FLipMouse](http://www.neilsquire.ca/latest-news/technology-news/lipsync-update-flipmouse-swap/) used. This device requires a much smaller range of motion. The pressure sensors are 3D printed, and thus lower the cost.

However, that does lead to one problem. Because the pressure sensor is printed, the printing has to be precise. They are quite small, and even small printing mistakes or inaccurate placement could change the amount of force needed.

We will keep you updated on the final joystick.

