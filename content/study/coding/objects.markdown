+++
title = ""
date = 2018-09-09T00:00:00
lastmod = 2018-12-30T00:00:00

draft = false  # Is this a draft? true/false
toc = true  # Show table of contents? true/false
type = "docs"  # Do not modify.
[menu.coding]
  name = "Objects"
  weight = 7
+++



# Coding [objects](objects.html)

## `babyobject`

`<obj>`

### General Orientation

This code captures the times that the baby is manually engaged with an object. 

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62793/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62793/download?inline=true>

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62777/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62777/download?inline=true>

Coders score only when object events occur, not when they don't occur. 
This is an event code, where gray spaces between cells mean that the baby is not engaged with an object. 

### Value List

`o` = object

`.` = when baby is off camera and coder cannot determine whether baby has an object in hand.

### Operational Definitions

`<obj>`

Object = is defined as any manipulable, moveable item that may be detached and moved through space (e.g., toys, household items, and smaller moveable elements of larger objects like beads on busy box, doorknob).

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62763/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62763/download?inline=true>

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/63765/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/63765/download?inline=true>

Objects may include large objects (i.e., a stroller, adult furniture, door, etc.) when baby moves them, thus, manually engaging with them. 
If the object never moves (e.g., the baby has a hand on the stroller but does not displace it), then this is not coded as 'o.'

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/63763/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/63763/download?inline=true>

The displacement rule is so that we can differentiate object engagement episodes from instances where baby is exploring a surface or resting hands on a surface for support.

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/63767/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/63767/download?inline=true>

The infant does not have to be looking at the object for the event to count as an object engagement (e.g., baby is carrying object).

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62775/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62775/download?inline=true>

Riding on toys with wheels does not count as object, but this will be coded in babyloc pass.

Code 'o' if the baby is engaged with an object by making contact with the item with hand(s) and/or moving the item in space (e.g., carrying, pushing on the floor, etc.) 

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62783/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62783/download?inline=true>

Onset is the frame when baby first causes the object to move while making contact with any part of the hand(s), not feet. 
Contact could be from any part of the hand (fingers, palm, side of hand). 
Movement could including lifting, holding, pressing, grasping, shaking, banging, or any other type of displacement event. DO NOT code onset, just when the hand touches the object if the object is not displaced (e.g., if they child touches a pillow but then 1 minute later actually grasps and moves it, code onset at the movement not when the hand touches the object). 
Offset is the frame when baby is no longer in manual contact with an object for at least 3 s. OR when the baby is in manual contact but the object is no longer being displaced (displacement includes holding, lifting) for at least 3 s. 
There is no minimum duration for baby to touch an object to be scored as 'o,' but if infant is touching multiple objects, the offset of 'o' object cell is when baby is no longer in manual contact with the last object contacted for 3+ s. 
If the baby is in manual contact with an object in one hand and makes contact with another object with their second hand, count this as the same bout. 

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62755/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62755/download?inline=true>

### How to Code

Set “JUMP-BACK-BY” key to 3 s.

Enable cell highlighting.

Watch in real time for the baby's hand(s). 
As soon as you see the hand(s) touch an object (as defined above), continue watching for a couple of seconds to see if the baby moves/manipulates the object. 
Then, hit #4-SHUTTLEBACK to get to the onset of the cell. 
The Onset is the first frame when the baby makes manual contact with the item. 
Set this onset by hitting ENTER to set a new cell with that onset time. 
Now, continue watching the object bout in real time and set the Offset when the baby breaks manual contact or stops moving object (e.g., stroller) for at least 3 s. 
Once you've determined that the bout has ended, set the offset by hitting #5-STOP and then #4-SHUTTLEFORWARD or #6-SHUTTLEBACK to the last frame where the baby is no longer in manual contact with the item and/or when the baby is no longer moving it. 
Then, hit #9-SETOFFSET.

Continue watching in real time for the next object bout. 
If the baby is holding an object while crawling or walking around, you can watch faster by SHUTTLING at 2x speed to find the end of the object engagement.

To check whether a 3-s pause has occurred between object engagements, go to the offset of the previous object cell and watch until you reach the next instance of 'o'. 
Then, hit the 'JUMP-BACK-BY' key and check to see if the previous cell lights up. If it does, then the two cells are <3 s apart and should be combined into one bout of 'o'.

## `momobject`

`<obj>`

### General Orientation

This code captures the times that the mom is engaged with an object. 
Coders score only when object events occur, not when they don't occur. 
This is an event code, where gray space in between cells means that the mom is not engaged with an object.

### Value List

`o` = object.

`.` = when mother is off camera and coder cannot determine whether she has an object in hand.

### Operational Definitions

`<obj>`

Object = is defined as any manipulable, moveable item that may be detached and moved through space (e.g., toys, household items). Object can include parts of a stationary object (e.g., doorknob on door, clasp on drawer) that can be moved or manipulated.

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62767/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62767/download?inline=true>

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62781/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62781/download?inline=true>

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62791/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62791/download?inline=true>

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62781/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62781/download?inline=true>

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/62797/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/62797/download?inline=true>

Object can include large objects that mom may move (chairs).

Code 'o' if mom is engaged with an object by making contact with the item with her hand(s). 
Onset is the frame when mom first makes contact with hands. Offset is the frame when mom is no longer in manual contact with an object for at least 3 s. 
If the mom has multiple items in hand, the Onset of object is when a hand(s) touched the first object in the multiple-object-bout and the Offset is when the hand(s) release the last object.

In cases of larger objects (i.e., a stroller, a box, a chair, a table, etc.), the object engagement begins when the object starts to move. If the large object never moves (e.g., the mom has a hand on the stroller but does not displace it), then this is not coded as 'o'.

</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/-/asset/63366/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/-/asset/63366/download?inline=true>

If the mom is not in the camera view, code this with a '.' as missing data.

### How to Code

Set “JUMP-BACK-BY” key to 3 s.

Enable cell highlighting.

Watch in real-time for the mom's hand(s). 
As soon as you see the hand(s) touch an object (as defined above), continue watching for a couple of seconds to see if the mom moves/manipulated the object (which would make this an instance of Object). 
Then, hit #4-SHUTTLEBACK to get to the onset of the cell. 
The Onset is the first frame when the mom makes manual contact with the item and moves it through space. 
Set this onset by hitting ENTER to set a new cell with that onset time. 
Now, continue watching the Object bout in real time and set the Offset when the mom breaks manual contact or stops moving the object for at least 3 s (i.e., Object bouts that are interrupted by gray space are more than 3 s apart.

There is no necessary minimum duration for object engagement during the 'o' bout to be coded as Object. 
In other words, the mom can engage with an item or as little or as much time as they would like, however, the mom must make manual contact and move it through space to count.

Once you've determined that the bout has ended, set the offset by hitting #5-STOP and then #4-SHUTTLEFORWARD or #6-SHUTTLEBACK to the last frame where the mom if no longer in manual contact with the item and/or when the mom is no longer moving it. 
Then, hit #9-SETOFFSET.

Continue watching in real time for the next object bout. 
If the mom is walking or crawling with an object, watch at 2x speed.

Do not agonize. 
If the mom goes in and out of the camera view, but you know she is still holding the same object and has not put it down, code it in the same bout of 'o'. 
Do not mark the “.” for every few seconds she is out of frame.

Code as Object event if mom's back is to the camera, but you see her arms moving and she overtly appears to be manipulating something—even if you can't see exactly what it is.

Many times, onsets and offsets are coded when mom goes in and out of frame. 
In these instances, hit the _0_ key to set a continuous cell, whose onset is 1-ms after the previous cell.
