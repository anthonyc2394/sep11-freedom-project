# Choosing My Tool
##### 11/07/22

In this blog entry, I will be discussing how I chose my tool for my freedom project. The tool that I chose was [Earsketch](https://earsketch.gatech.edu/landing/#/learn) which allows users to create music using Python or Javascript. My end goal for my freedom project is to create a music platform where people can create their own music and apply visuals to their work. The music platform would also save your work so you can edit your work instead of starting all over, since I want to work with someone that is learning [Firebase](https://firebase.google.com/).

I haven't really tinkered with Earsketch, since there is a lot to learn still, but some of the things I learned were:

* `fitMedia()` is a function that adds a soundclip that you can modify using parameters
* The format is `fitMedia(parameter1, parameter2, parameter3, parameter4)`
* `parameter1` represents the sound clip chosen
* `parameter2` represents the track number
* `parameter3` represents the start measure (when the sound clip starts)
* `parameter4` represents the end measure (when the sound clip ends)

* `makeBeat()` is a function that adds a rhythms that you can customize using parameters
* It follows the same format as `fitMedia()` except for `parameter4`
* `parameter4` represents the beat string (duration of the rhythm and when it pauses)

For example:

```js
setTempo(120);

fitMedia(RD_UK_HOUSE_MAINBEAT_8,1,1,5);
fitMedia(RD_POP_PADCHORD_2, 2, 1, 9);

// Fills
var fillA = "0---0-0-00--0000";
var fillB = "0--0--0--0--0-0-";
var fillC = "--000-00-00-0-00";
makeBeat(OS_SNARE03, 3, 4, fillA);
```

The line `fitMedia(RD_UK_HOUSE_MAINBEAT_8,1,1,5);` means that the sound clip `RD_UK_HOUSE_MAINBEAT_8` will be added to track 1 , starting at measure 1 and ending at measure 5.

The line `makeBeat(OS_SNARE03, 3, 4, fillA);` means that the sound clip `OS_SNARE03` will be added to track 3, starting and ending at measure 4 following the rhythm pattern of `var fillA = "0---0-0-00--0000";` where the `0`'s represnt when the rhythm plays and where the `-` reprsents when it pauses

Right now, I'm at step 0 of the Engineering Design Process because I haven't defined a problem yet and hvae only researched my tool for the past few weeks.

Some skills that I used during the past few weeks were How to learn and How to Google. I used the How to learn skill by remembering how I learned my SEP10 tool the best. Last year I learned best through videos and visual examples, so I used the How to Google skill to find good video tutorials that help me learn Earsketch using Javascript and not Python.

[Next](entry02.md)

[Home](../README.md)