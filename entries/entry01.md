# Choosing My Tool
##### 11/07/22

In this blog entry, I will be discussing how I chose my tool for my freedom project. The tool that I chose was [Earsketch](https://earsketch.gatech.edu/landing/#/learn) which allows users to create music using Python or Javascript. My end goal for my freedom project is to create a music platform where people can create their own music and apply visuals to their work. The music platform would also save your work so you can edit your work instead of starting all over, since I want to work with someone that is learning [Firebase](https://firebase.google.com/).

I haven't really tinkered with Earsketch, since there is a lot to learn still, but some of the things I learned were:

*
*
* `fit.Media()` adds a sound

```js
setTempo(120);

function addSection(clips, drums, beat, lead, segLen, start, length) {
    var track = 3;

    for (var n = 0; n < length; n++) {
        makeBeat(drums, 1, start + n, beat);
    }

    for (var c = 0; c < clips.length; c++) {
        fitMedia(clips[c], track, start, start + length);
        track += 1;
    }

    if (lead) {
        generateLead(segLen, start, length);
    }
}

function generateLead(segLen, start, L) {
    var leadClips = [RD_EDM_RAVELEAD_1, RD_EDM_RAVELEAD_2, RD_EDM_RAVELEAD_3, RD_EDM_RAVELEAD_4, RD_EDM_RAVELEAD_5, RD_EDM_RAVELEAD_6];

    var numSegs = Math.floor(L / segLen);

    for (var n = 0; n < numSegs; n++) {
        var r = Math.floor(Math.random() * 6);
        fitMedia(leadClips[r], 2, start, start + segLen);
        start += segLen;
    }
}

var clips1 = [RD_EDM_RAZORBASS_2, RD_EDM_ANALOGLEAD_4, RD_EDM_ANALOGPLUCK_2];

var clips2 = [RD_EDM_CHORDPART_5, RD_EDM_PERCSYNTHLEAD_1, YG_EDM_FX_12];

var clips3 = [RD_EDM_CHORDPART_5, RD_EDM_PERCSYNTHLEAD_1, YG_EDM_FX_12, RD_EDM_SFX_RISER_1];

var drums = [OS_KICK02, OS_SNARE04, Y24_FX_2, Y24_ELECTRO_2, OS_OPENHAT05];

var beat1 = "0430322-12-13223";
var beat2 = "0+1+0+110+1+0111";
var beat3 = "0+++0+++0+++0+++";

addSection(clips2, drums, beat3, false, 1, 1, 4);
addSection(clips3, drums, beat2, true, 2, 5, 4);
addSection(clips1, drums, beat1, true, 0.5, 9, 4);
addSection(clips1, drums, beat1, true, 0.25, 13, 4);
addSection(clips2, drums, beat3, true, 1, 17, 4);
addSection(clips2, drums, "", false, 1, 21, 4);

// Effects
var pan = [0, 0, 50, -50, -35, 35];
var vol = [0, -1, 0, 0, 0, 0];
for (var i = 0; i < 6; i++) {
    setEffect(i + 1, PAN, LEFT_RIGHT, pan[i]);
    setEffect(i + 1, VOLUME, GAIN, vol[i]);
}
```

Right now, I'm at step 0 of the Engineering Design Process because I haven't defined a problem yet and hvae only researched my tool for the past few weeks.

Some skills that I used during the past few weeks were How to learn and How to Google. I used the How to learn skill by remembering how I learned my SEP10 tool the best. Last year I learned best through videos and visual examples, so I used the How to Google skill to find good video tutorials that help me learn Earsketch using Javascript and not Python.

[Next](entry02.md)

[Home](../README.md)