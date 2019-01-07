+++
title = ""
date = 2018-09-09T00:00:00
lastmod = 2018-12-30T00:00:00

draft = false  # Is this a draft? true/false
toc = true  # Show table of contents? true/false
type = "docs"  # Do not modify.
[menu.coding]
  name = "Coding setup"
  weight = 2
+++

# Coding Set Up

This section describes how to transcribe & code the 1-hour natural play session.

## Getting Started

Download the [development version of Datavyu](http://datavyu.org/download.html).
Download the `PLAY_CodingTemplate.opf` file from the [PLAY Databrary Volume](https://nyu.databrary.org/volume/254/slot/14924/-?asset=73892). 
Name this file with the PLAY naming convention (e.g., PLAY_NYU001, … PLAY_NYU010, … PLAY_NYU030).
  - This template contains all of the primary variables that will be coded by each site: communication, gesture, object interaction, locomotion, and emotion.
Download Ruby scripts for each coding variable as needed from the [PLAY Github repository](https://github.com/databrary/PLAY-Project-Datavyu-scripts).

## Get to Know Datavyu

Familiarize yourself with Datavyu before you begin coding (resources on Datavyu.org, videos from past workshops, etc.).
Refer to the [Datavyu User Guide](http://www.datavyu.org/user-guide/index.html).
Take a look at our [Best Practices for Coding Behavioral Data From Video](http://www.datavyu.org/user-guide/best-practices.html) on the Datavyu site.

## Coding in Passes

The coding manual describes the [transcription ](transcription.html) process and codes for 5 content areas: [communication](communication.html), [gesture](gesture.html), [object interaction](objects.html), [locomotion](locomotion.html), and [emotion](emotion.html).
Each content area includes two passes: one pass for the infant and one pass for the mother. For gesture, the baby and mom are coded together in a single pass.
A pass entails scoring the relevant codes for 1-hour of video.

    Please visit our GitHub Repository <https://github.com/databrary/PLAY-Project-Datavyu-scripts> for all of the scripts mentioned in this wiki.
    
## Workflow for Coding Communication Passes

After the file has been transcribed according to procedure in Transcription, run two additional scripts that will prepare new Communication columns for further coding.
Run `splitmombaby_transcribe.rb`. This script pulls out mom and baby language from the transcribe column into two new columns: (1) momspeech and (2) babyvoc. 
Each column is automatically populated with cells from the respectively tagged utterances from the transcribe column (e.g., the script ports all utterances coded as ‘m’ to the momspeech column and 'b' to the babyvoc column). 
Each new cell in momspeech and babyvoc is a point cell created at the onset of each cell from the transcription.
Run create_mombaby_utterancetype.rb. 
This script also creates two new columns: (1) momutterancetype and (2) babyutterancetype. For each cell in momspeech and babyvoc, a new cell is created in momutterancetype and babyutterancetype, respectively. 
The codes for these cells are blank, and the coder now scores mom and baby communication according to definitions in Communication Codes.

## Workflow for Coding Gesture Pass

Score baby and mom gesture together in a single pass according to definitions in Gesture Codes.
After the gesture coding pass (for both mom and baby) has been done, run a script that will separate mom and baby gestures into two columns.
Run `Split-MomBabyGesture.rb`. This script pulls out mom and baby gestures from the gesture column into two new columns: (1) babygesture and (2) momgesture. Each column is automatically populated with cells from the respectively tagged events from the gesture column (e.g., the script ports all gestures coded as ‘m’ to the momgesture column and 'b' to the babygesture column). Each new cell in babygesture and momgesture is a point cell created at the onset of each cell in the gesture column.

## Workflow for [Object](objects.html), [Locomotion](locomotion.html), and [Emotion](emotion.html) Passes

Choose whether to code baby or mom first within each pass for object, locomotion, or emotion.
Score each pass according to definitions in Object Codes, Locomotion Codes, or Emotion Codes.
Workflow for Inter-Observer Reliability on Communication, Gesture, Object, Locomotion, and Emotion Passes
After the primary coder finishes a pass: babyutterancetype, momutterancetype, gesture (split into babygesture, momgesture), babyobject, momobject, babyloc, momloc, babyemotion, or momemotion run two scripts to set up the Datavyu spreadsheet for coding reliability.
First, run a script called `insert-RelBlocks.rb`.
This script randomly generates 3, 5-minute chunks within the first, second, and third 20-minute sections of the 1-hour video of free play. By quasi-randomly inserting reliability blocks from areas of the primary coder’s pass, this will ensure that the reliability coder sees each portion of the video for each child’s session. Thus, the idiosyncrasies of each child, fluctuations over the 1-hour session, and drift in the coder are spread over the session.
Reliability on each coding pass is done on the same 3, 5-minute blocks for each pass.
The scripting window in Datavyu will prompt when everything has been successfully completed. You should now have a brand new column in your spreadsheet named reliability_blocks.
This script should only be run once so that reliability coding can be done within the same time frame for each coding domain for each session.
Now, run another script appropriate for the pass reliability needs to be coded on: `CreateReliability-BabyUtterancetype.rb` or `CreateReliability-MomUtterancetype.rb` or `CreateReliability-Gesture.rb` or `CreateReliability-MomBaby-Loc.rb` or `CreateReliability-MomBaby-Object.rb` OR `CreateReliability-MomBaby-Emotion.rb`
This script inserts new coding columns where your reliability coder will score the video while they are locked into the script-generated, 5-minute chunks in the reliability_blocks column.

# Coding ID

Datavyu ID Code for 1-Hour Natural Play

    Make sure you are currently logged in at Databrary to view embedded video examples in this wiki.
    
## id

`<site>` `<participant>` `<testdate>` `<birthdate>` `<agegroup>` `<sex>` `<study>` `<babylanguage1>` `<babylanguage2>` `<momlanguage2>` `<momlanguage2>`

### Operational Definitions

`<onset/offset>`: Set every ID cell onset to 00:00:00:000 (hours : minutes : seconds : milliseconds).

Set ID cell offset to the last frame in the 1-hour free play session.

`<site>`: Site refers to the data collection site: New York University, Rutgers Newark, CUNY Staten Island, Penn State, etc.

Get the site from the metadata information collected on the app.

Format is three letters all caps: NYU, RTG, CSI, PSU.

`<participant>`: Participant number refers to the infant's participant number in the order that the data were collected.

Participant numbers run consecutively from 001 within each site.

Get the participant number from the metadata information collected on the app.

Format for id number is three digits 001, 012, 021.

`<testdate>`: Test date is the day of the home visit.

Get the test date from the metadata information collected on the app.

Format for test date is YYYY-MM-DD.

`<birthdate>`: Birth date is the day the baby was born.

Get the birth date from the metadata information collected on the app.

Format for birth date is YYYY-MM-DD.

`<agegroup>`: Entered as 12, 18, or 24.

Get the age group from the metadata information collected on the app.

`<sex>`: Refers to infant's biological sex.

Code `m` = male/boy; `f` = female/girl.

Get the sex from the metadata information collected on the app.

`<study>`: Study name.

Code as 'PLAY'.

`<babylanguage1>`: Refers to infant's predominant language spoken during the session.

Code with lowercase, full name of the language: 'english' or 'spanish'.

`<babylanguage2>`: Refers to infant's other language spoken during the session, if another language was spoken.

Code with lowercase, full name of the language: 'english' or 'spanish'. If no other language was spoken as missing '.'

`<momlanguage1>`: Refers to mother's predominant language spoken during the session.

Code with lowercase, full name of the language: 'english' or 'spanish'.

`<momlanguage2>`: Refers to mother's other language spoken during the session, if another language was spoken.

Code with lowercase, full name of the language: 'english' or 'spanish'. If no other language was spoken as missing '.'
