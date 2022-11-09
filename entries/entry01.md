# Choosing My Tool
##### 11/07/22

In this blog entry, I will be discussing how I chose my tool for my freedom project. The tool that I chose was [Earsketch](https://earsketch.gatech.edu/landing/#/learn) which allows users to create music using Python or Javascript. My end goal for my freedom project is to create a music platform where people can create their own music and apply visuals to their work. The music platform would also save your work so you can edit your work instead of starting all over, since I want to work with someone that is learning [Firebase](https://firebase.google.com/).

I haven't really tinkered with Earsketch, since there is a lot to learn still, but some of the things I learned were:

* `fit.Media()` is a function that adds a soundclip that you can modify using parameters

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

The line `fitMedia(RD_UK_HOUSE_MAINBEAT_8,1,1,5);` means that 

Right now, I'm at step 0 of the Engineering Design Process because I haven't defined a problem yet and hvae only researched my tool for the past few weeks.

Some skills that I used during the past few weeks were How to learn and How to Google. I used the How to learn skill by remembering how I learned my SEP10 tool the best. Last year I learned best through videos and visual examples, so I used the How to Google skill to find good video tutorials that help me learn Earsketch using Javascript and not Python.

[Next](entry02.md)

[Home](../README.md)