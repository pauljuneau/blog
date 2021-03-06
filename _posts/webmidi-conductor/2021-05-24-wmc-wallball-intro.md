---
layout: post
title: Webmidi-Conductor Wallball Game Introduction
date:   2021-05-21 06:40:00 -0700
categories: webmidi-conductor
permalink: /:categories/:slug:output_ext
tags: webmidi-conductor games wallball
comments: true
---
Introduction to the [webmidi-conductor javascript opensource repo](https://github.com/pauljuneau/webmidi-conductor) in action via a wallball pong game demo.
<!--end_excerpt-->

<iframe width="560" height="315" src="https://www.youtube.com/embed/vwvn2FGb3Rc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Wall Ball Game Demo Overview
[Click Here to Play!](https://www.pauljuneauengineer.com/webmidi-conductor/)

#### Introduction
The video above is a demonstration of [my open source JavaScript library](https://github.com/pauljuneau/webmidi-conductor) I wrote that processes live midi input to determine if notes being played are within the designated scale along with identifying triad or 7th chords. I created a simple wall ball variation of the classic pong game to show how the player's paddle can react to midi input in real-time to move the paddle based on scale progression or change its color based on chord detection. The library can also use live audio input to detect changes in pitch which moves the paddle up/down in this game demo, or computer keyboard input can be used to simulate playing on a small piano. The computer keyboard to piano key mapping is defined in the ReadMe of the webmidi-conductor GitHub repo.

Hope you enjoy! Thanks for checking this out! 
#### Setup 

* Plug in your midi instrument (e.g. piano) to your computer or smartphone prior to accessing the game demo site via link above.
   * In the video above, I used a Yamaha Digital Piano P-45 connected to a Samsung S10 phone via a midi usb cord.
      * refer to the [official Yamaha P-45 downloads page](https://usa.yamaha.com/products/musical_instruments/pianos/p_series/p-45/downloads.html) for midi driver software and manuals for iOS device compatibility, midi reference, and an owner guide. 
         * _Note: I am not affiliated with Yamaha in any way._ 

#### Rules

* Playing up or down in pitch causes paddle to move up or down.
* Paddle will shrink if not playing within the designated scale.
* Goals are 10 points 
   * Wall must be hit enough times to make the wall disappear in order to score a goal.
* Triad chords are 3 points & 7ths are 4.
* Wall color is based on the defined key's position on the Circle of 5ths mapped to the corresponding color position on a RGB Color Wheel.
   * C Major/A Minor is Red, E Major/C# Minor is Green, and G# (Ab) Major/F Minor is blue.
   * ![RGB Color Wheel](https://www.w3schools.com/colors/pic_rgb_wheel.gif)
   * ![Circle of Fifths](https://upload.wikimedia.org/wikipedia/commons/thumb/3/33/Circle_of_fifths_deluxe_4.svg/600px-Circle_of_fifths_deluxe_4.svg.png)
* When chord is played, paddle will change color to related chord's key mapped to RGB Color Wheel based on the key's position on the Circle of 5ths.
   * C chords are red, E chords are green, and G# (Ab) chords are blue.

----
#### webmidi-conductor blog contents
{% include wmc-links.html %}
{% include wmc-blog-content.html %}
