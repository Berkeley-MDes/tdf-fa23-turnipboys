# Report #7 - Week of 10/12/2023

## Aylish Turner

### Reflections

We did a lot this week! After receiving some feedback from Shm on our initial "CleanTech" idea, we decided to pivot and just focus on designing a system of Photons that could communicate with one another. The final product would then emerge out of that.

Our re-designed concept: Ghosty, the Hot/Cold game! Ghosty is a little ghost that is scared of the light. When the lights are on, it'll run away until it finds a dark place to hide. Using your "ghost catcher" tool, you play a game of Hot/Cold to see how close you are to Ghosty and catch it!

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/DESINV%20202%20-%20Ghosty%20storyboard%201.png)

We created a [Figma](https://www.figma.com/file/iTPrt7UdsSuKgONyTlIzIG/Wipey%3A-TDF-Project-2?type=design&node-id=7%3A2&mode=design&t=EmpagBOGm7JHa7A0-1) to keep track of our design process. 

Christine was out of town so most of the initial programming and design was completed by Ankur and I, but we made sure to keep Christine up to speed. She had some valuable input and designs later in the week once she returned!

First, we decided to experiment with the Photons and see if we could even get some motion happening. On Shm's recommendation, we followed the [Accelerometer --> Servo tutorial](https://github.com/Berkeley-MDes/tdf-fa23-equilet/blob/main/project_demonstrables/particle_workbench/accel_to_servo/README.md). 

When you tilt the accelerometer (which is attached to the breadboard), it changes the direction and speed of the Servo motor. Our biggest challenges were just learning what kind of functions to call upon from the in-built Servo library. However, we were successful and managed to get the motor going!

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/10_12_23%201.jpg)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/accelerometer_1.gif)

This was great because it meant we could figure out how to modify the code to get continuous motion from light input rather than the accelerometer. However, after attempting to modify the accelerometer code, we ran into some roadblocks. We did some additional external research to learn more about the Servo and figure out how we could just get continuous motor motion.

In order to get continous motion, we found [this tutorial](https://docs.idew.org/internet-of-things-project/references-for-wiring-and-coding/continuous-rotation-servo-motor) and followed it, with some small changes.

First, because we had a different Servo motor, we connected our Servo motor to the 3.3V pin and NOT the V-USB pin (for 5V). If you don't use the 3.3V pin you'll fry the Servo. Our code didn't seem to be working, which I didn't understand. Then, I realized that it was probably the motor itself and suggested we swap them out. Thankfully, it worked after that! :) RIP fried Servo!

After that, we just adjusted the variable to fit our needs for continuous motion.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/continuous%20motion.gif)

Finally, we needed to put it all together. We want the ghost to "run away and hide" in the light, so we combined Sudhu's LED light input code with our Servo motion code. Now, when the sensor picked up a certain level of light, the motor would start moving. Once it reached a certain level of darkness, the motor would stop.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/light%20input%20motion_2.gif)

Ankur experimented a bit more with the ultrasonic distance sensor, but we agreed that it likely wasn't the best choice to try and measure distance between the ghost and the ghost hunter because the ultrasonic sensor was just measuring the distance of any object in front of it.

Christine began speculating about how to actually fabricate the ghost robot to get the wheels moving.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/10_12_23%20christine%20design.jpg)

Unrelated to all of that, my dad and sister came to visit me and went to SF to see the sea lions. :) So happy :)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/10_12_23%20pier%2039.jpg)

### Speculations

This type of technology already exists, but I think that it might interesting to see it applied more to children's games and safety. For example, playing Hot/Cold with your child at the playground and having a little tracker on them just in case. I was a child put on a leash, so anything to escape the Elmo leash...lol.

I also think that this could be very cool when combined with other AR elements. It could make Pokemon Go feel a lot more realistic, for example, if you had a Pokedex (your phone?) that led you on more of a chase than the current app does.

Our current biggest challenge seems to be the actual robotics manufacturing of it, since I know very little about constructing mobile robots.
