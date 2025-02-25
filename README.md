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