---
layout: project
title: Checkers Playing Gantry
permalink: /projects/checkers-playing-gantry/
type: Embedded Systems
description: A 3-axis gantry designed with the purpose of manipulating board game pieces.
tags:
  - Embedded C
  - Controls

repo_url: "#"
demo_url: "#"
image: "/assets/images/SLDWORKS_eQYhpWy82Z.png"
placeholder: PCB / scope image
---

## Overview
This progress project aimed to apply the topics I learned in MAE 6194 - Mechatronics. I aimed to design and build robot a that can play checkers.
s
## Technical Information
I used TMC2209 stepper motor drivers and AS5600 magnetic position encoders communicating over I2C for feedback motor control. Each Nema-17 Stepper motor had its own Arduino nano running proportional control with a naive motion planning algorithm which scales the velocity with error. These were controlled by a main computer (Raspberry pi 5) sending position commands via UART over USB.

## Outcomes
Due to time constraints, I was only able to complete the linear motion system. This was what I expected to complete within the timeframe. It is still significant, since the other two axes of motion are the same system as the first.

## Lessons Learned
I knew going into this project that time would be a concern, however, I should have made the project scope smaller into something like an automated camera slider. An automated camera slider would utilize the same motion system, but with less overall complexity.

Additionally, a majority of the project time was spent on fabricating the frame. Starting the project earlier would alleviate this issue.

The 3D printed gear was sometimes slipping on the shaft of the motor due to high resistance, in future projects I should be more careful with material choice and alignment.

## Showcase
<div class="project-inline-video">
  <iframe
    src="https://youtube.com/lD-X4mhh2e8"
    title="Linear Motion System"
    loading="lazy"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
</div>