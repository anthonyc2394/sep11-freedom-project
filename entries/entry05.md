# Entry 5
##### 04/23/23

### Content

In this blog entry, I will be walking you through the process of me finishing the mvp of my freedom project and the next steps for my project. For 2 months, I've been focused on one song made entirely made with [Earsketch](https://earsketch.gatech.edu/landing/#/learn). I started of by using Earsketch sound seach engine to listen to guitar and piano sounds from different genres (pop, hip hop and rnb) and I would favorite the, so it would be easier to find it later on.

Some of my favorite sounds are:

* `AK_UNDOG_PIANO_3`
* `RD_ELECTRO_DRUMROLLBREAK_6`
* `Y21_KEY_3`

After looking over my favorites I decided to use piano sounds, but I still had no idea how I would structure my song and the sounds I would use. I started off with `AK_UNDOG_PIANO_3`, but I didn't want it to start like that, so I decided to search the artist, Alicia Keys, to find sounds that would fit with the piano. I came across vocals such as `AK_UNDOG_OOHS_AHHS_4` and `AK_UNDOG_OOHS_AHHS_1` to create vocals for the intro 

```js
// Loops
for (var measure = 9; measure < 25; measure += 2) {
    fitMedia(AK_UNDOG_PERC_KICK_2, 4, measure, measure + 1)
}
for (var measure = 10; measure < 25; measure += 2) {
    fitMedia(AK_UNDOG_OOHS_AHHS_1, 4, measure, measure + 1);
}
```

From there I just added sounds that made the song better (drums, vocals and more) and I finished it.
The code for the entire song is [here](https://github.com/anthonyc2394/freedom-project-mvp/blob/main/script.js)


The next steps for my freedom project si to create a pop song and then start creating visuals (videos) using [p5js](https://p5js.org/) for each song. So far I've been looking at this [documentation](https://p5js.org/examples/sound-load-and-play-sound.html) to see if my idea is possible, but I haven't tried it yet.

### EDP

Right now, I'm on steps 5, 6 and 7 of the Engineering Design Process

### Skills

creativity
time management

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)