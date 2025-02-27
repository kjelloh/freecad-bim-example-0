# freecad-bim-example-0

## Please consider to support the creator of the original tutorial!
* Free Download the 2D Drawings and Sketches :  https://ko-fi.com/s/5caaf65d22
* If you want, you can purchase the FreeCAD File too :  https://ko-fi.com/s/b49b41474a

This Github repo contains my documentation and created files of following youtube video "FreeCAD 2025 BIM - Architecture - Complete Beginner Tutorial" (https://youtu.be/IV-nv9ygZPM ).

![](/images/image-0.png)

## Consider my experience and 'good to know' from doing the tutorial in Freecad 1.0 om my Macbook Pro M3 14" 18 GB?

	==> Zooom in and out is 'two fingers up or down on the trackpad" (Touchpad navigation setting)

![](/images/image-1.png)

Zooom in and out: 'two fingers up or down on the trackpad"
Translate view: <Shift> + one finger on track pad
Rotate view: <Option> + one finger on trackpad
 

	==> 'Create Building' starts a new tree structure with 'Building' as the root

![](/images/image-2.png)    --> ![](/images/image-3.png)

Note: I renamed the Budiling to 'House' by editing its 'Label'


	==> 'Create Level' is used to create a 'floor' and I need to drag-and-drop it under the 'Building' root

![](/images/image-4.png)  --> ![](/images/image-5.png)

Note: I renamed the Level by editing its 'Label'.

	==> 'Split Edge' is required to actually split (a line point does not automatically split an edge / line)

![](/images/image-6.png)

Note: 'Slit Edge' is a submenu of 'Trim Edge' in <Sketcher Tools>.


	==> Consider to Select items before clicking on a 'Constraint'?

I tried to click 'Constraint Coincident' and then two 'points' but had a hard time making the constraint take effect.
![](/images/image-7.png)

Maybe it works better if I first select the two points and then click the constraint (like the presenter does in the video)?

	==> 'Close sketch' seems to be in the upper right corner?

![](/images/image-8.png)

Note: The <Close> button seems to be in the 'Tasks' panel BUT: The 'Tasks' header shows only when hovering with the mouse over this panel (possible confusion).

![](/images/image-9.png)

The 'Tasks' panel header as shown when hovering over it with the mouse.

    ==> Click on an edge to select a 'planar shape' for the 'Slab' tool!

	==> Click on an Edge to select a 'Planar Shape' for use with the 'Create Slab' tool

![](/images/image-10.png)

Note: It does not seem to work to click inside a shape to select it (like in Fusion 360)?

    ==> I wonder why the presenter draws the wall 'from scratch' without referencing the 'Slab'?

	==> It seems we need to drag-and-drop the created 'Slab' into the 'Level' container to impose our project topology?

	==> It seems the 'Sketch' used for the 'Slab' gets put under the 'Slab' in the tree?

![](/images/image-11.png)

Note: I did not expect this and wondered where the sketch went?


	==> I wonder why the presenter draws the wall 'from scratch' without referencing the 'Slab'?

	==> The 'Offset' tool looks like an old ink pen?

![](/images/image-12.png)

==> The 'Add offset constraint' of the 'Offset Geometry' tool parameters is a little opaque (and unexpected)?

![](/images/image-13.png)

It seems the 'Add offset constraints' inserts something that looks like construction lines that allow us to later change (access) the set constrains?

![](/images/image-14.png)

Question is why this is an option and not always there (like in Fusion 360 where you can always access previous operations parameters)?

	==> It seems a 'Symmetric constraint' between a line and a point is to place the point at the center of the line?

I expected a 'symmetric constraint' to involve three items. The two items to be 'symmetrically constrained' and the item two witch the two items are symmetric. Why is this not so here? A 'symmetric constraint' between an end point of the construction line of the offset constraint on one hand, and the edge line or the other, does not translate to placing the end point at the center of the edge in my head?

	==> It seems after closing the sketch all construction lines and measurements are made invisible (only plain lines show)

I am confused so much of the sketch 'disappears'  when I close it?

	==> The 'Wall' tool operates on the whole sketch (not a shape like in Fusion 360)

	==> The presenter in the video does NOT extrude a sketched wall, but a sketch inner perimeter + a wall widths

I wonder why he did not sketch the wall cross section and then extrude it like I would have done in Fusion 360?

Also, By applying the Wall tool to the inner perimeter we have to repeat the 20 cm wall thickness we already sketched. What if we change the sketch to indicate a thicker wall? Then this will NOT affect the actual Wall created by the tool? This kind of rubs me the wrong way?

==> The tutorial requires the user to have the exterior wall plans to place them 'unguided' (on their own)

![](/images/image-15.png)

This is the front exterior wall plan


![](/images/image-16.png)

This is the back side exterior wall plan

![](/images/image-17.png)

This is the right exterior wall plan

![](/images/image-18.png)

This is the left exterior wall plan


![](/images/image-19.png)


The House I had created up to the point of guided in detail by the presenter in the video 


	==> To add the remaining windows and doors was like struggling with an annoying puppy...

Although you select to create a 'door' you get an option pane for a 'window' which seems how it is supposed to be?

Editing the width and height of a 'window' is a bit tricky. If you try to scroll the option pane you often accidentally change some other value by having the cursor placed over the value edit box (scrolling inside a value box 'scrolls' the value). Also, the value is not selected when clicking in the value box. And if you hit <Ctrl>-A to select 'all' and enters a value it will be interpreted as millimeter. You have to remember to re-add 'cm' for centimeters to have the value be correct. This is a bit strange as we have set the 'default' in the FreeCad 'Preferences' to 'cm'?

I also managed to get a lot of 'garbage' sketches and windows outside the container where I was working (the EXT WALL container). I am not sure why but it seems any failure to commit any window creation leases 'half baked' or 'residue' windows and sketches? Well, I was able to delete them manually at least.

The 'type' of window or door to create was confusing. Looking at the video it seems all doors should be of 'glass' which seems to correspond to the type 'fixed'? I am not sure. It seemed like a guessing game.

The placing of 'windows' (doors and windows) was tricky. Sometimes I managed to align with an existing window or door upper frame by enabling 'snap endpoint' in the 'Draft' tool pane plus pressing 'z' to lock the movement to the z-axis. But it was not easy and often ended with a failure (and the residue sketches and windows was created in the items tree).  

	==> Still, with some patient I was able to create doors and windows that at least looks like the ones in the video?

![](/images/image-20.png)

My house after having created and placed all remaining windows and doors (all glass).


	==> A 'Hole Depth' for a door may cut through more than the wall the door is placed on (s t r a n g e)!

The video points out we need to address this problem by changing the 'Hole depth' from 0,00 cm to 10 cm! And in this way (somehow) the 'Hole Depth' is reduced?! Now this is of course totally unprofessional behaviour of a CAD tool...

![](/images/image-21.png)

Note: The presenter explains that this behaviour comes from 'the walls' not being separate walls. But in fact a 'single wall'. I suppose this comes from us creating the interior walls from a single sketch? Still, for some reason this behaviour was not observed when I created the doors to the side rooms? Why did those doors not cut also the opposite walls? Strange...

	==> I had a problem with the first opening (the 115 cm wide one to the left)

The internal wall plan sketch had the correct width of 115 cm from the inside wall to the internal wall center line.

![](/images/image-22.png)

But this means the actual opening is 110 cm in my drawing. I failed to figure out why the presenter does not mention that a 115 cm opening is 5 cm to large? That is, if I have somehow generated the internal walls incorrect as 'centered'. Still, the other larger opening fits with my opening so centered walls seems ok there? Anyhow, I changed my 'left opening' to 110 cm.

	==> It seems selecting an 'opening' does not show in the view (that is, I fail to see any highlighting of the selected opening)?

Maybe a plain opening has 'no substance' and therefore has nothing to be highlighted? Still, it is confusing...

	==> The 3D/BIL tool ribbon 'Roof' tool applies to a whole sketch.

	==> It seems if I enter a bad formatted value in the 'Roof' properties dialog its contents disappear?

I am in Sweden so I tried entering '6,5' degrees roof slope (but I needed to enter '6.5' with '.' decimal separator otherwise the content disapperaed).

I tried entering '30 cm' for roof thickness (but this seems invalid as the dialog content went invisibale).

Note: The fix was to close and open (double click)  the 'Roof' item again.


	==> On macOS <Command> + <click> allows for selecting multiple items in the items tree. 

	==> I succeeded to cut the external and internal walls to the roof.

![](/images/image-23.png)

My house looked like this after having finished the roof (before adding backside slab and front and back stairs)

	==> It seems we should create a flight of Stairs with NO sketch or other item selected? 

I had folder 'INT WALLS' selected. Then when I clicked the 'Stairs' tool in the '3D/BIM' tool bar a 'Stairs' folder was created outside the folder. BUT - no stair could be seen in the view of the house? But if I clicked the 'Stair' tool with no item selected, then a default stair was created at origo.

![](/images/image-24.png)

The default flight of stairs created at origo when clicking the 'Stair' tool in '3D/BIM' tool bar while NO item in the items tree was selected.

	==> It seems a flight of stairs with 'Number of steps' set to 4 shows 3 steps?

![](/images/image-25.png)

A 'Stairs' object with 'Number Of Steps' set to 4 shows a flight of stars with 3 steps?

	==> Command+C and Command+V on macOS works for 'copy-and'paste' on the 'Stairs' object in the tree view.

	==> AHA! Objects are NOT 'Dragged and Dropped' but 'Selected-and-moved'!

Until this point I had tried to 'drag-and-drop' objects when using the 'Move' tools. But this is NOT how to use them. You have to 1) Select the object to move. 2) Click the 'Move' tool button. 3) Click a reference point on the object to move. 4) Then select the reference point on the target where to move to. That is, you shall NOT hold down the mouse button while moving the object! Took me a while to figure out...

	==> I now have the whole 3D house modelled and organised into a top folder '3D MODEL'

![](/images/image-26.png)

My house 3D model so far.

![](/images/image-27.png)

The 3D model as a top folder with the root folder 'House' in it.


	==> It seems the 'Section Plane' tool is in the 'Annotation Tools' tool bar?

![](/images/image-28.png)

The 'Annotation tools' tool bar


![](/images/image-29.png)

The 'Section Plane' tool in the  'Annotation Tools' tool bar.

	==> It seems the 'Section Plane' is shown in the view as a green plane?

![](/images/image-30.png)

A created section plane at z-height 100 cm.

	==> It seems the presenter sugests we projekt the selected objects to the XY-plane (as opposed to create a 'cross section')?

![](/images/image-31.png)

	==> It seems we move the created 'Shape2DView' with right click and then click 'Transform' (NOT use the 'Move' tool)?

![](/images/image-32.png)

The 'Transform' tool to translate the created 'Shape2DView'.

Note: The semantics is a little opaque to me here. Why is this a 'view' and not 'a thing' like a drawing or a projection or what have you. A 'view' indicates it will change with changes to the 3D model? Maybe?

	==> AHA! At 45:27 the presenter discovers the error in width of the left inner wall opening (that I already fixed above) :)

![](/images/image-33.png)

In the generated floor plan the presenter discovers the notch into the wall due to the 'too wide' opening (that I already fixed in my model above) :)

	==> It seems 'showing the swing plan' of doors is a property of the door itself (and not of the generator of the floor plan)?

![](/images/image-34.png) ![](/images/image-35.png)

By setting 'Symbol Plan' of each door property it shows up on the created 'Shape2DView' with an accompanying  a 'swing path'

AHA! They show up also in the 3D model! So that is way they show also on this 2D 'view'?!

	==> The presenter sugests I draw the floor plan in the 'TechDraw' workbench.

![](/images/image-36.png)

The 'TechDraw' workbench in the Workbench drop down.

Note: At this stage it is a bit strange that we have the 'view' just sitting around beside the 3D model...?

Why is the work flow not to create a 'drawing' directly. That is, have the 'view' project directly into a separate 'thing'?

	==> It seems we now finally actually create a 'page' for the floor plan drawing?

![](/images/image-37.png)

The 'Insert Default Page' in the 'TechDraw' workbench.

Note: The semantics here seems to be that we first have a 'view' created in the 3D view. Then we create a 'Page' to put the view on? Well, lets see...

	==> It seems we use the 'Insert View' with the 'Shape2DView' selected in the model tree?



![](/images/image-38.png)

The 'Insert View' in the 'Techdraws Views' tool pane.

![](/images/image-39.png)

Note: The semantics is again a bit vague? The 'Insert View' tool is a member of the 'TechDraw' workbench that takes a 'Shape2DView' as an argument? But where is it inserted? I imagine we can have several 'Pages' created in (by?) the 'TechDraw' workbench? 

Also, the 'Shape2DView' is still some strange unknown thing sitting around in the 3D view... 

Well, let's continue!

	==> It seems the font size for 'Dimensions' are set to 20 cm by default?

![](/images/image-40.png)

The presenter showed how inserted dimensions in the 'Page' with the 'View' is by default HUGE!

And they were also for me. This is unprofessional! 

Is the semantics here that the font is measured in the same scale as the thing we are viewing? That is, the 3D model of the house is many meters. So a label with a font size of 20 cm will look just fine in 'real life'? Well, I find this confusing? I mean, we are 'drawing' a 'view', not the real object?


	==> It seems to be several Issues with the Font and Stability of the 'Page' Dimensions?

My font for Label and Dimensions looked strange and was clipped.

![](/images/image-41.png)

It turned out that my macOS FreeCad 1.0 came with a 'TechDraw' workbench default font was 'Academy Engraved LET' (and that made measurement text be clipped).

![](/images/image-42.png)

I changed to 'Arial'

![](/images/image-43.png)

...

	==> OK - My FreeCad on macOS (Apple Silicone) is really unstable in 'TechDraw' and 'Page' edit!

Dimensions become 'inactive' and uneditable (although I can continue creating new ones)

Often the all the tools in 'TechDraw' workbench (or is it tools for the 'Page') gets inactive (and I have to restart FreeCad to get them usable again)

The 'Apply Geometric Hash to Face' often refuses to show a dialog.

![](/images/image-44.png)

For now this feature in FreeCad 1.0 on macOS Apple Silicone is BROKEN! ...

