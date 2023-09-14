# Report #3 - Week of 9/14/2023

## Aylish Turner

### Reflection

#### Class Recap

Thank you to TJ and Jeff for helping to explain Grasshopper and its visual scripting system a little better to me. I think that I'm so used to it being one or the other - strictly 3D modeling with meshes like Maya & Blender, or strictly programming C#/Python/whatever in an IDE that I'm having a hard time navigating Grasshopper. However, the explanation of panels, arrays, lists, and other components helped a lot. I had to restart my project multiple times due to Rhino/Grasshopper issues (such is life) but I am glad that I experienced it this early on so I know how to handle it at this point.

#### Lost in the Sauce...

Most of this week was spent procrastinating and dreading the final deliverable because I honestly wasn't sure about what I wanted to do. I wanted to customize my phone stand to be very personal and fun, but experimenting with Rhino and Grasshopper was very difficult for me since I am still very new to the software.

I think that I've grown a lot and already improved my knowledge quite a bit (especially considering I had never even heard of Rhino/Grasshopper before we downloaded it), but I was worried that my skills weren't enough to really power through the project and turn in something interesting.

I finally decided to just sit down and try something out, which was extremely difficult but definitely a good learning experience.

#### Restrictions

I wanted to start a new project, completely fresh. This was very very scary to me and a part of why I kept putting it off - I wasn't really confident in my skills and prioritized other projects I knew I could be somewhat successful in. 

I prioritized just learning as much as I could and trying to showcase what knowledge I did gain in the process, even if the final product was pretty bad in the end and I ended up switching gears entirely.

My goals:

- Explore as much of Rhino, Grasshopper, and Illustrator as I can.
- Create a custom phone stand using Rhino and Grasshopper.
- 3D print the phone stand (my first time using a 3D printer) or laser cut the stand (my first time laser cutting on my own).
- Optimize the phone stand for vertical orientation; useful for video calls, filming, and mindless Reddit scrolling (lol).

### The First Project - 3D modeling, Rhino, and Grasshopper

#### Inspiration

I thought that it would be very funny to create a phone stand modeled around *2001: A Space Odyssey.* My phone would be the monolith with an ape on one side and a bone on the other.

![](https://mediaproxy.salon.com/width/1200/https://media.salon.com/2013/07/2001_monolith.jpg)

[Image description: A frame from 2001: A Space Odyssey depicting the apes looking at the monolith.]

#### Design

My phone would be completely vertical, which is an unusual position for a phone stand but useful for my filming purposes. It also emulates the monolith better, which is my primary goal.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/DESINV%20202_phone%20stand%20design%20copy.png)

[Image description: My concept design of the phone stand.]

I initially planned for the phone stand to be quite wide and thin, with enough support to hold the phone up vertical. I also considered leaving room for a charger wire on the bottom, but that would make the stand very tall and I didn't really want that, so I later scrapped it. I wanted the phone to seem tall and foreboding rather than it looking like a bunch of tall rocks stacked on top of each other.

#### Process

I was honestly having so much trouble with this. I thought that I had a decent grasp of Grasshopper basics but nothing I did really seemed to work. My objects wouldn't cap properly (or so it seemed) and I was running on very little sleep, so nothing made sense to me. I also had fallen ill this week, but I wanted to push through and see how much I can learn about computational modeling.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/first%20attempt%20gh.PNG)

My first attempt at constructing just some basic cylinders stacked on top of each other as a basic stand bottom.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/why.PNG)

But when I uploaded my baked & exported model to Sketchfab, it was just the cylinders???? They were not solids???? Something went wrong here in my exporting process...

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/progress%202.PNG)

I made a little bit of progress with my cylinders and managed to fix the cap issue (not even sure what happened with the first attempt), but I was struggling with the solid difference component. I followed TJ's directions from his tutorial video and watched many videos online, but I couldn't figure out what I was doing wrong. I think that I'm missing some kind of vital step about the breps or some plane or something at the start of my Grasshopper file, but I will need to ask for extra assistance to figure it out.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/second%20attempt%20gh.png)

[Image description: My Grasshopper program for reference.]

SOLID DIFFERENCE ISSUE: Still not sure how to do it in the way TJ did it, but I believe by adjusting the length/height of my rectange I could get it almost flush with the other cylinders. So that fixes it, at least partially.

#### Issues

Nearing the wire, it came down to a combination of factors, but mostly a really big one:

- I became really, really sick. It began at the start of the week and it might have just been stress or maybe I caught something, but I was super exhausted all of the time and really quite ill. I wasn't really sure what "level" this project would be for me since I came in going "Rhino? Grasshopper? So many animals..." and now I have learned a ton, but I was a little too caught worrying about the details of what is "exceeding" or "meeting" expectations. I imagine that this is probably a level 1 Triceratops project, but I really couldn't be sure.

#### Putting a Pin in It

Here is my collection of resources because I REALLY want to continue finishing this. Maybe in the next couple of weeks I can just turn it into a personal project. I don't even like *2001* that much. I just really want to complete this because it was an interesting challenge and I know that once my brain is all healed & rested I can definitely do it!

[TJ's video on the simplified phone stand](https://www.youtube.com/watch?v=GHtWNAPiAoE)

[General Grasshopper tutorial that is EXTREMELY good and very clear](https://www.youtube.com/watch?v=zDDVeDldvaI)

[Tutorial on how to shape rocks in Rhino](https://www.youtube.com/watch?v=q92OS1llRt0)

[Landscape contour using Noise4D tutorial (for the sandy/rock texture)](https://www.youtube.com/watch?v=sR4jOSznkYo)

[Texture displacement in Grasshopper](https://www.youtube.com/watch?v=f74fiNWkxVw)

[Procedural textures, noises, rocks](https://www.grasshopper3d.com/forum/topics/rocks)

### Project 2: So...What Now? (Continued 3D modeling)

I made some small changes to TJ's simple phone stand file. First, I put in my phone's dimensions and specified that I wanted a portrait orientation. Then, I adjusted the spheres until I found a nice spherical shape. I made sure to leave an opening at the bottom of the sphere so that I could pull my charger cable through. I also created an additional cylinder (or more accurately, subtracted a cylinder) on the back of the stand so that I can store my Surface Pro stylus pen.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/simple%20stand%20v2.1.PNG)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/simple%20stand%20v2.2.PNG)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/simple%20stand%20gh.png)

This is my Grasshopper file for this stand. You can see where I have some disabled components from testing out different cylinders and shapes to create a space for the charging port.

#### A Little Textural Fun

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/bubblewrap%20stand.PNG)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/cloud%20stand.PNG)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/fire%20stand.PNG)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/shadow%20stand.PNG)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/strawberry%20stand.PNG)

Playing around with some weird textures. 

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/2023-09-14%2008-35-56_1.gif)

[Link to Sketchfab](https://skfb.ly/oLpX9) where I uploaded my 3D model.

#### Printing

Finding time to print was very challenging, despite my attempts to print for several days. My project is quite large and would have taken at least 13 hours according to the Prusa printer estimates. I also have to be honest that while I would really like to 3D print something, I found the phone stand that I made rather ugly (LOL) and would rather save the material for something else. I still hadn't laser cut anything on my own (I laser cut once with a friend for another class) so I thought that that might be an exciting activity to round out my experimentation and learning for the week.

### Project 3: Laser Cut

#### Design

I wanted to laser cut something. I already had my customized phone stand from a few weeks ago that I had baked and exported into an AI file, but I never ended up cutting it earlier. I decided that it was finally time.

I customized the AI file to make it a little cuter - I went through a lot of ideas, but thought that a little bunny stand would be fun. I've used Adobe Illustrator in the past, but that was at least 6 years ago. After my initial confusion at the updated interface, I found myself back in the swing of things.

Here is the original phone stand after baking it in Grasshopper and exporting in Rhino:

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Phone_stand_layout.PNG)

And here is my version (bunny style):

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Project%201_laser%20cut%20phone%20stand%20v2%20AI%20file.PNG)

#### Laser Cutting

I was nervous about completing my first laser cut, but I had already observed a lot of my friends cutting and received some great advice from the instructors and Makerspace staff, so I felt prepared. And it ended up being a lot of fun!

Materials:

- 1/4" plywood
- Adobe Illustrator file
- Jacobs Hall laser cutter

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Project%201_Laser%20cut%20gif.gif)

On my first cut, I accidentally switched the base and back plates, so what was supposed to be the bunny's head ended up being the bunny's feet & vice-versa. I also forgot to adjust for the size of the plywood I was using, so none of the pieces fit into each other (thank you to Yunting for advising me on this!). 

After some semi-quick edits, I fixed the layout and did a second cut, which was far more successful! I then did one more just in case. I am so pleased with the results! It's super simple but also very recognizable and I received a lot of positive feedback from other people in the Makerspace.

![What the pieces look like immediately after the laser cut is completed](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Project%201_lasercut%20img%201.jpg)

[Image description: What the pieces look like immediately after the laser cut is completed.]

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Project%201_lasercut%20img%202.jpg)

The two final bunny phone stands that I cut out! The one on the right is the second attempt and the one on the left is the third attempt. I'm pretty pleased with the results!

#### Polish

The bunny phone stands are already super cute in their simple plywood form, but I wanted to add a pop of color (I was mostly just tired of looking at plain wood, white models, etc.). I also haven't painted anything in a while, so I thought that it would be a nice opportunity to crack open some of my tubes and brushes.

First, I washed all of my pieces. They were still covered in ash and lasercut stains from the cutting process which was getting all over my hands and clothes. A lot of articles online recommended using white vinegar to gently dissolve and clean the ash off, but I didn't have any so I just used gentle soap, water, and a soft cloth face towel.

![The pieces after being washed.](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Project%201_lasercut%20after%20cleaning.jpg)

[The pieces after being washed.]

I was a little bit worried about the paint layer being too thick because then the pieces wouldn't be able to fit together, so I did thin layers of paint and then a thin layer of modge podge to give it a shiny look.

Here are the completed phone stands!

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/20230914_144938.jpg)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/20230914_144946.jpg)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/20230914_145023.jpg)


# Report 2 - Week of 9/7/2023

## Aylish Turner

### Reflections

#### Review & Familiarization

This week was mostly a "Get to know Rhino and Grasshopper a little better" week. 

I encountered an issue with Rhino where I suddenly couldn't select any of my objects. This mystified myself as well as some other students, but after assistance from all three instructors, we found out that my Default layer had somehow become locked! This made it as to where I couldn't select or drag any objects I had baked onto that layer. I'm not sure how it became locked, but it's something that I look out for now.

In class last week, Dr. Sudhu demonstrated how to use the laser cutters and gave some good advice on how to move the laser cutter around our material. This was a very helpful demonstration that made the concept a bit less intimidating. Now I would like to experiment more with the 3D printers.

I also found TJ's ["Computational Design: Worked Example"](https://youtu.be/GHtWNAPiAoE) video very helpful. I had never heard of the term "computational design" before, but applying that term to the type of 3D modeling that Rhino does made it a lot more clear. I'm used to programs like Maya and Blender, which also have computational design elements, but are a little more freeform in their style of 3D modeling and animating. Thinking about modeling from a mathematical perspective is very interesting and something I had never considered before, since I usually just kind of "go with the flow" and consider it a very tactile experience. 

Otherwise, I have scheduled an appointment to use the laser cutters and will also take additional 3D printing trainings so that I can experiment a little more and improve my in-class design. 

#### Speculations

Rhino could be very helpful for some of my other class projects. I could see myself utilizing the 2D laser cut patterns for my Studio Foundations potted plant design. It might also be helpful for printing out robotic parts, although my robotics knowledge is severely lacking. Right now I just need to come up with some more modifications to personalize the phone stand. I am a bit nervous to mess it all up, but I've re-started the project files so many times now that I'm kind of past the initial fear.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/20230907_103552.jpg)
(Image description: Some designs for my Studio Foundations projects that might be interesting to print or laser cut patterns into. I wonder how thin vs. thick the materials should be if I like the end result to be cylindrical (for laser cutting). Maybe I can score the wood or other material after?)

#### TLDR;

Not a ton of updates, mostly just increasing my familiarity with the program and watching a lot of tutorials. More exciting pictures incoming next week as I modify and print my design!

# Report 1 - Week of 8/31/2023
## Aylish Turner

### Reflections

#### The Basics
This week, I started learning how to use Rhino and Grasshopper for the first time. My main goals were to learn the fundamental tools and vocabulary of the program, then to customize the Project 1 example files for my phone dimensions. If I had time, I wanted to prep the files for laser cutting and print for the next class.

First, I followed the [Rhino Tutorials](https://www.youtube.com/watch?v=V67fq8eCY8A&list=PLWIvZT_UEpWXp1ZYFiQ01w2nf4HApO09t&index=2) linked on the course Wiki. This was extremely helpful because I realized that many of the terms and tools were simlar to other 3D modeling programs I have used in the past, like Maya and Blender. This helped simplify the concepts for me and made Rhino/Grasshopper seem less intimidating. I also watched the [Grasshopper Tutorials](https://vimeopro.com/rhino/grasshopper-getting-started-by-david-rutten) by David Rutten. (As a side note, Rutten's audio was very difficult to hear and understand, but the explanations were actually very good).

At the very end of this report, I will have a list of Rhino and Grasshopper "quick tips" that really helped me. I'm adding these as an easily searchable reference guide.

After reviewing these interface basics, I decided to try modifying the Project 1 Cell Phone Stand files.

#### Modifying the Cell Phone Stand Files

I worked in the CellPhoneStand_all Rhino file. There were a lot of different viewports and I couldn't figure out how to dock all of them (I only seemed to have a maximum of 4 viewports at once, so some were free-floating). I am a big fan of the Rhino Command line. It makes searching within Rhino sooo much easier than other programs. 

After opening up Grasshopper, I got to work modifying the Cell Phone Stand parameters. I was modifying them directly within the Grasshopper components instead of the Remote Control Panel, so next time I want to work within the Remote Control Panel since I imagine it's a lot faster. But starting with just panning around the many components and nodes of Grasshopper was really helpful because I could see how everything connected.

I measured the dimensions of my phone, a Samsung Galaxy S20 FE 5G. I chose to measure my phone with the case still on, since that's how I use my phone every day.

I used a T-square to measure the dimensions in cm and then converted to mm. Due to the pop socket attached to the back of the phone case, the dimensions are likely slightly off.

- Length: 165 mm
- Width: 80 mm
- Depth: 18 mm (with pop socket)
- Phone screen offset from edge: 5 mm

While measuring, I listened to an episode of the "Stretch and Fade" podcast.

<img src="https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Phone_case_measurements_8_31_23.jpg"  width="270" height="480" />
(Image description: A black phone case with a Buc-ee's pop socket measured by a T-square.)

After inputting my custom measurements, I also changed the student's height to my height, 1600 mm.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/phone_measurements_8_31_23.PNG)
(Image description: A screenshot of Grasshopper parameters that specify phone dimensions.)

Once I had modified all of the applicable dimensions, I decided to follow [TJ's baking guidelines](https://docs.google.com/presentation/d/1ZdU7iIDoGudH3jucSfdLrt5zrcxYz4Oy5nLrqNIxCa4/edit#slide=id.g240a16639ea_0_0) so that I could create a 2D layout for laser cutting. 

This was a slightly confusing process for me at first because one of the components was highlighted orange to notify a warning (lack of geometry to bake). I then realized that I had the 3D model box checked, so I unchecked that and then baked both curves. I followed the remaining steps as described in the guide to export an Adobe Illustrator file and a PDF version of my phone stand's 2D layout.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Phone_Stand_Capture_8_31_23.PNG)
(Image description: A Rhino window capture displaying the 2D phone stand layout objects.)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Phone_stand_layout.PNG)
(Image description: The phone stand layout as exported in PDF form.)

### Speculations

My next goals for this project are to prep my 2D layout for laser cutting and then to laser cut my phone stand. I would also like to export the 3D model version so that I can try 3D printing the phone stand.

I don't know much about parametric modeling or the Rhino software, but I see a lot of similarlites to Unreal Engine, which seems to be getting better with each update. The processing power of Unreal is very impressive and a lot of game, film, and themed entertainment studios are utilizing it for professional development spanning across modeling, lighting, animating, and programming. 

A potential future development could be creating 3D scans of objects through image capture that can then be uploaded to Rhino as editable objects. There are ways to do this, but I wonder how the process could be simplified, perhaps by using AI that can estimate dimensions based on the quality of the image capture and its environment (I have done something similar to this in the Snapchat Lens Studio with AR filters).

I have also used a very interesting tool that is quite different from Rhino but also plays with a combination of 2D and 3D space in a very interesting way. [Mental Canvas](https://mentalcanvas.com/) is a tool for drawing 2D images in a 3D space, giving the illustrations more depth with a parallax effect. I tried this out a couple of years ago and really enjoyed it. There are a couple of different payment options as well as a free trial promo.

Here's a YouTube video that demonstrates some of Mental Canvas's capabilities, "Biomimicry" by Giuliana Flavia Cangelosi:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=a2RuG3BHvY4" target="_blank"><img src="http://img.youtube.com/vi/a2RuG3BHvY4/0.jpg" alt="Video thumbnail of detailed trees" width="240" height="180" border="10" /></a>

### Rhino & Grasshopper Quick Tips
- Viewport quick tips:
    - double-click viewport name tab to maximize the view
    - double-click again to go back to minimized view with all 4 viewports
    - when maximized, hold CTRL & then use the TAB button to cycle through the views
    - right click: rotate view
    - Shift + right click: pan view
    - Ctrl + right click: zoom in & out
    - mouse wheel: zoom in & out on steps
- Display modes:
    - different options for how Rhino displays the objects (i.e. wireframes, shaded, rendered, etc.)
- Geometry:
    - points
        - have no volume
        - do not represent 3D shape
        - just X,Y coordinate
    - curves
        - created by placing points in space
        - lines, conics, & freeform curves
        - control points determine shape & location of curve in space
    - surfaces
        - already have an extension in 3D space
        - surfaces have control points
    - polysurfaces
        - a compound of single surfaces joined together by their edges
        - allow for more complex shapes
        - no control point access
        - edited through solid tools tab
    - subD objects
        - subdivision
        - more sculptural modeling process
        - faces, edges, & vertices
        - can be modified by editing these elements
    - meshes
        - generated from sculptural geometry
        - composed of flat polygons
        - higher polygon count = higher fidelity of curved object
            - i.e. fewer polygons = more jagged look; more = more smooth
- Selection methods:
    - drag a window from right —> left: everything within/touching window is selected
    - drag a window from left —> right: everything FULLY within window is selected
    - shift + click to add to selection
    - ctrl + click to remove from selection
    - selection brush allows you to draw your selection area
        - ctrl & shift keys adjust radius of brush
