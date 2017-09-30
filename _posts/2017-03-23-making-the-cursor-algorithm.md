---
layout: post
title: Making the Cursor Algorithm

---

Over the past few months I’ve kept you updated on the progress of our hardware, our trials and errors in the process of physically building a LipSync, but I’ve said little about the progress of the software — the coding that will actually cause the cursor on the screen to move, from the input of the joystick movement.

Well, today, I’ll explain the decisions we’ve made from the coding perspective. There will be a bit of math, a few graphs, but what we’re talking about is how the cursor on the screen moves — and why it moves like it does.


<img src="http://www.neilsquire.ca/wp-content/uploads/2017/03/linear-function.jpg" title="A linear function"/>
<em><strong>A linear function, which is used to create an algorithm that directly connects the cursor speed to the amount the mouthpiece is moved. (All of these are rough sketches).</strong></em> 

Initially, we had decided to program the cursor with an algorithm based on a linear function. In English, this means that the cursor would move just as much as the joystick is pressed. This means it wouldn’t speed up and down based on the amount of pressure applied by the user on the joystick, but rather, it would remain at a consistent speed.

To get a picture of what I mean, contrast that with a computer mouse. A computer mouse speeds up and down depending on how much you move it thanks to the acceleration programmed in (to see the effect of acceleration on your mouse speed, turn off “enhance pointer precision,” which turns off acceleration, in your mouse settings). However, a joystick is different than a mouse.

While the mouse can theoretically have unlimited movement, a joystick has a finite — limited — amount of movement, the amount you can push it in any direction. While a mouse only moves the cursor as you physically move the mouse, a joystick will move the cursor until you let go of it (if you hold it down to the right, for example, it will continue moving right). Thus, acceleration is harder to program on a joystick.

So initially, the cursor only moved in direct relation to the movement of the joystick. But this was tedious. While moving small distances was tolerable, it would be a pain dragging the cursor from one side of the screen to the other. As well, it created a blocky effect, as it was unable to move in a purely circular motion.

<img src="http://www.neilsquire.ca/wp-content/uploads/2017/03/logarithmic-function.jpg" title="A logarithmic function"/>
<em><strong>A logarithmic function, which we thought would make a greater range of speed possible.</strong></em> 

So we decided that the function needed to be more complex, after some internal testing. With a logarithmic function, theoretically, the cursor’s speed would be more variable, depending on where on the screen the user needed to go — if they needed to go a short distance, it would go slow as they moved the joystick less, and if they needed to go far on the screen, the cursor would move fast as the joystick was pushed to the edge.

But there was a problem — it was too fast. While the linear function produced an algorithm that was tedious and slow, the logarithmic function created a cursor too fast to control. The “sweet spot” that would allow you to move it slow was just too small, and most of the time you would have overshot anything. Because the cursor was so fast — and you were overshooting your target with the cursor — it would take longer to do anything on your device than with the linear algorithm.

We had overlooked the need for smaller movements with the cursor. In order to use a LipSync with a cursor coded with the logarithmic function, you would have to be precise — it would be a steep learning curve, and not that intuitive.
 
<img src="http://www.neilsquire.ca/wp-content/uploads/2017/03/exponential.jpg" title="An exponential function"/>
<em><strong>Above: An exponential function, which we are currently using to program the cursor.</strong></em>

<em><strong>Below: All three functions, for comparison.</strong></em> 	
<img src="http://www.neilsquire.ca/wp-content/uploads/2017/03/all-three-functions.jpg" title="All three functions"/>
With a little bit more work, we had come up with a solution — an exponential algorithm. With this function, when the joystick is pushed to the extreme edge, it is capable of a fast-moving cursor, but unlike the logarithmic function, there is a more diverse range of speed in the slower range of movement.

Essentially, it goes slow when it needs to — when a small distance is needed, like using the text editor — and it goes fast when the user expects to go faster. It’s much more intuitive.

And unlike the linear and logarithmic — which was so fast it created a herky-jerky effect — functions, the movement is smooth.

However, we are still figuring some details out, as we work to make the LipSync as easy to use as possible. We are still tweaking the max speed of the cursor — how fast it could possibly go — and the slope of the function — which would alter the behavior of the mouse, like how much pressure would make it go fast, and how little would make it slow.
