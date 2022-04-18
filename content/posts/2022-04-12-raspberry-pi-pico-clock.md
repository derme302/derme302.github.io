---
title: "Raspberry Pi Pico Clock"
date: 2022-04-12T13:11:00+10:00
draft: false
---
![Pico Clock](/uploads/2022/04/pico-clock.png)

I was reminded about a very cool clock that sits on my desk after a [kind Tweet from Matt Trentini](https://twitter.com/matt_trentini/status/1507951632687898627). It's been working so well that I almost forgot I built it.

<!--more-->

During the great COVID pandemic I had a lot of time for side projects and I came across this wonderful project on Reddit by Dr2Mod. He had designed and built a Solar System clock that showed the current time and position of the planets. You can find the [GitHub Project here.](https://github.com/dr-mod/pico-solar-system)

After a few weeks of sourcing components, with all the supply chain issues, I finally got the clock assembled.

This is where I ran into some slight issues. This clock is based on the [Raspberry Pi Pico](https://www.raspberrypi.com/products/raspberry-pi-pico/), which is an ARM microcontroller board the foundation has released for embedded electronics. So the chip requires some extra software to program it compared to a regular Pi. This was mainly an issue for me as I don't have a bare metal Linux machine and I had to pass the device through to my virtual machine.

Once I got the utilities installed and Pi connect to my VM the rest of the process was relatively painless. 

The simulation is written in [MicroPython](https://micropython.org/), which is a partial implementation of Python 3 for embedded systems. 

Twelve months on the clock is still working perfectly with zero issues, which honestly surprised me. My past experience with systems like this with screens is that they are very prone to memory leaks. I think this shows the potential of MicroPython for projects like this. Which is why I am looking for to playing with MicroPython more in the future.
