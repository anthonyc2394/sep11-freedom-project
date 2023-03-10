# Tinkering With My Tool
##### 02/11/23

### Content

In this blog entry, I will be discussing what I have learned and practiced within the past few months from [Earsketch](https://earsketch.gatech.edu/landing/#/learn). I learned how to use `for loops` and how to add custom sounds on Earskecth.

#### Loops

Similar to how artists can play a pattern repeatedly using a loop pedal, programmers can instruct the computer to perform actions repeatedly using a `for loop`. A `for loop` is a loop that repeats until a specified condition is false. A `for loop` takes in 3 components: initialization, condition and afterthought.


Below is an example of a `for loop` from [Earsketch](https://earsketch.gatech.edu/earsketch2/?curriculum=8-0-0&language=javascript)

``` js
var drum1 = OS_SNARE03;
var beat_string = "0---0---0-0-0---";

// Looping our beat
for (var measure = 1; measure < 5; measure++) {
    makeBeat(drum1, 1, measure, beat_string);
}
```

This code would loop the sound `OS_SNARE03` and make it have the pattern `0---0---0-0-0---` starting from measure 1 till the condition is false (when measure is = 5).


#### Custom Sounds

Custom sounds is a feature on Earsketch that allows you to create and add new sounds to Earskecth. You can add up to 30 seconds of a music file you want to use or have created by clicking the add sound button and uploading the file.

When you want to use the new file, you should use the following format:

``` js
setTempo(120);

fitMedia(username/beatname, track number, start measure, end measure);
```


### EDP

Right now, I'm at step 0 of the Engineering Design Process because I haven't defined a problem yet and have no idea what to create, but I'm hoping that in my next entry I will have answers.

### Skills

Some skills that I used during the past few weeks were How to learn and How to Google. I used the How to learn skill by remembering how I learned my SEP10 tool the best. Last year I learned best through videos and visual examples, so I used the How to Google skill to find good video tutorials that help me learn Earsketch using Javascript.

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)