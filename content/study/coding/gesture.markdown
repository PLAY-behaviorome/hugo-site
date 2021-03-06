+++
title = ""
date = 2018-09-09T00:00:00
lastmod = 2018-12-30T00:00:00

draft = false  # Is this a draft? true/false
toc = true  # Show table of contents? true/false
type = "docs"  # Do not modify.
[menu.coding]
  name = "Gesture"
  weight = 5
  
tags = ["gesture", "video"]
+++



# Coding [gesture](gesture.html)

## `gesture`

`<source_m-b>`, `<gesture_p-s-i-c>`

### General Orientation

Gestures are segmented, [durative](https://www.dictionary.com/browse/durative), event-based behaviors. 
Watch the video paying attention to the communicative gestures used by the parent and the child. 
When coding for gesture, focus on the mother’s or baby’s hands and head.

Code mother and baby gesture simultaneously in one pass. Then based on the `<source>` of the gesture, a script breaks apart mom and baby into separate babygesture and momgesture columns.

Only onsets are coded to expedite coding; offsets could be coded later if duration of gesture or overlap with specific other domains is of interest.

### Value List

`<source_m-b>`
`m` = mom
`b` = baby
`h` = mom holding baby

`<gesture_p-s-i-c>`
`p` = point
`s` = show/hold up
`i` = iconic gesture
`c` = conventional gesture

### Operational Definitions

`<source_m-b>`
`<m>`: Code 'm' if the mom is the source of the gesture.
`<b>`: Code 'b' if the baby is the source of the gesture.

`<gesture_p-s-i-c>`

Gesturing by either mom or baby to the investigator, or anyone else in the room, should not be coded. 
The following should NOT be coded as gestures: tapping baby to get his/her attention; pushing an object away; hugging and kissing; one partner moving the other's hand (e.g., to initiate contact, like proximity seeking); jerking the head to indicate “come here.”

`<p>`

Code 'p' when the baby or mom extends their index finder to indicate reference to objects, people, events, or locations in the environment.

Onset is the frame when the finger is fully extended in space toward a referent, or when the point finger is extended and makes contact with the object. 
Repetitive points should be coded as separate gesture events.

`<s>`

Code 's' when the baby or mom holds up an object to present it as if to say: “look at this” or “do you want this” or “I want you to take this”. 
Given that it’s not possible to distinguish intention, when a participant shows, offers, or gives an object (e.g., baby actually hands toy to mom, offering toy to mom but mom doesn’t take) code as 's', to save decision-making time.

Onset is the frame when the object is fully held up or out to show it. Repetitive instances of holding up or offering an object should be coded as separate gesture events.

`<i>`

Code 'i' when the baby or mom engages in an iconic gesture. 
They are called iconic because they represent an object, idea, or action that can't easily be referenced with a deictic (point/show) or conventional gesture. 
The movement of these gestures usually calls to mind something about the nature of the object, idea or action being referenced. 
For example, you could move your arms back and forth to represent running, or you could trace a square in the air with your finger, or flap your arms as if flying.

Onset is the frame when the baby or mom has clearly begun the iconic gesture, and the coder can clearly identify this a gesture but does fall into the conventional gesture category (see `<c>`). Repetitive instances of an iconic gesture should be coded as separate gesture events.

`<c>`

Code 'c' when the baby or mom engages in a conventional gesture. Conventional gestures are culturally-agreed-upon hand or head movements with a specific meaning, like nodding the head to mean “yes,” shaking the head to mean “no,” and moving the finger to lips to indicate “be quiet”.

shaking head “no”
</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/20618,23455/asset/76362/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/20618,23455/asset/76362/download?inline=true>

holding out hand for “give me”
</br>
<video width="320" height="240" controls>
<source src="https://nyu.databrary.org/slot/14765/20618,23455/asset/76362/download?inline=true" type="video/mp4">
</video>
</br>
<https://nyu.databrary.org/slot/14765/20618,23455/asset/76362/download?inline=true>

If a gesture is conventional, you should be able to understand its meaning just by seeing it in isolation, without knowing any of the context. 
Some additional examples of conventional gestures include: waving, clapping, flipping arms out to side to indicate “I don’t know’ or “where is it”, come here gesture (finger motions or palms), sit down gesture (pats ground), pickup gesture (child holds up arms to be picked up), thumbs up, shrugs, naughties (wag finger), hug me (hold arms out asking for hug), etc.

Onset is the frame when the baby or mom has clearly begun the conventional gesture, and the coder can clearly identify this a gesture but does fall into the iconic gesture category (see `<i>`). 
Repetitive instances of a conventional gesture should be coded as separate gesture events.

### How to Code

Set “JUMP-BACK-BY” key to 2 s.

Gestures are best coded with the volume low or muted so that the language content does not confound the coding process.

Watch in 1x speed until either mom or baby gestures. Focus on the mom’s and infant’s hands and head to identify instances of gestures.

Gestures are defined purely as they relate to the communicative nature of each action. The coder can establish whether something is communicative by looking at things like eye contact, conversational context, and the reaction of the person being spoken or gestured to. If the movement isn’t supposed to communicate anything, then it’s not a gesture. For example, a child might reach for an object and pick it up and look at it. This is an action, not a gesture. But, if the child points to the object to indicate its presence, or if the parent claps her hands to indicate “good job,” then these are gestures. (If there is significant ambiguity in whether a gesture is communicative, or how to code it, sound may be of assistance.)

When the coder identifies a mom or baby gesturing, jump back 2 seconds and play the video again at ½ speed until the frame the gesture is clearly underway is found. Hit the = key (equal sign) to insert a point cell; so the current video frame becomes the onset and the offset.

Type 'm' or 'b' to indicate whether mom of the baby was the <source> of the gesture. Hit the TAB key to advance the cursor to <gesture>, then type 'p', 's', 'i', or 'c' to indicate the type of gesture.

Splitting Mom and Baby Gestures
It's faster to code mom and baby gesture together in one pass. But for consistency with the other coding passes, we want mom speech and baby gestures to be in two separate columns.

Run the Split-MomBabyGesture.rb script to pull baby and mom gestures from the the gesture column into babygesture and momgesture columns.

## `babygesture`

`<gesture_p-s-i-c>`

### General Orientation

Contains gestures produced by the baby.

This column is automatically populated after the gesture pass is completed, using a Ruby script. All of the gestures tagged with 'b' in <source> in the gesture column are transferred here. The onset and offset are equal, and set to the onset from the gesture column, which reflects the time when the coder was sure the gesture had begun.

### Value List

`<gesture_p-s-i-c>`

`p` = point

`s` = show/hold up

`i` = iconic gesture

`c` = conventional gesture

## `momgesture`

`<gesture_p-s-i-c>`

### General Orientation

Contains gestures produced by the mom.

This column is automatically populated after the gesture pass is completed, using a Ruby script. 
All of the gestures tagged with 'm' in <source> in the gesture column are transferred here. 
The onset and offset are equal, and set to the onset from the gesture column, which reflects the time when the coder was sure the gesture had begun.

### Value List

`<gesture_p-s-i-c>`

`p` = point

`s` = show/hold up

`i` = iconic gesture

`c` = conventional gesture
