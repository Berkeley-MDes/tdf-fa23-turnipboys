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
