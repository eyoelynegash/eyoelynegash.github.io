---
layout: post
title: Portable Guitar Preamp
description: My Discovery Project, a small preamp with a three-band EQ for quiet practice
---

**Discovery Project** · Status: in progress, prototyping on a breadboard

## Overview

For my ECE Discovery Project, I'm building a small, portable guitar preamp so I can practice without playing through a loud amplifier. The build follows the [Portable Guitar Preamp](https://www.instructables.com/Portable-Guitar-Preamp){:target="_blank"} guide on Instructables and adds the [Tonemender](https://runoffgroove.com/tonemender.html){:target="_blank"} tone stack from runoffgroove, which gives me bass, mid, and treble controls.

<img src="{{ site.baseurl }}/assets/images/preamp-signal-flow.svg" alt="Signal flow diagram: guitar into a preamp input stage, then the Tonemender EQ with bass, mid, treble, mid shift and level controls, then the output">

## The problem

I wanted to practice guitar at home without disturbing my family. A full amplifier is loud, and turning it all the way down usually makes the tone thin and lifeless. Commercial headphone amps exist, but I wanted to understand how a guitar signal is shaped, not just buy a box that does it for me. That made it a good engineering problem: design something small and portable that still sounds good at low volume.

## The process

**Research.** I started by studying existing designs. The Instructables guide gave me a proven, portable preamp to start from, and the Tonemender gave me a well-documented tone stack. The Tonemender uses a dual op-amp and has Bass, Mid, Treble, and Level controls, plus a Mid Shift switch. That switch moves the center of the midrange dip to about 400 Hz or 700 Hz, so the same circuit can sound closer to a Fender-style or a Marshall-style amp.

**Prototyping.** Instead of soldering everything right away, I'm building the circuit on a breadboard first. This lets me test each stage on its own, swap parts, and fix mistakes without desoldering. My experience assembling harnesses at Roytec taught me how much easier it is to catch a problem early than after everything is permanently connected.

**Learning along the way.** This project connects directly to what I'm studying. Working with op-amps, filter networks, and gain staging has given me a practical feel for concepts like frequency response and signal levels that can seem abstract on paper.

## The outcome so far

The design is chosen and the prototype is underway on the breadboard. My next steps are to:

1. Finish testing each stage and confirm the tone controls behave as expected
2. Measure the frequency response and compare it with the published Tonemender curves
3. Move the circuit to a permanent board and fit it in a small enclosure
4. Use it for real practice sessions and note what I'd change in a second version

## What I learned

The biggest lesson so far is that a good design starts with understanding the problem, not the parts list. Building on proven designs let me focus on understanding why each part of the circuit matters. I'll update this page with photos, measurements, and final results as the build comes together.

*Circuit references: the Portable Guitar Preamp guide on Instructables and the Tonemender by runoffgroove. The signal flow diagram was made by me.*
