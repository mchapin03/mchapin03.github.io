---
layout: project
title: Rube Goldberg Machine
permalink: /projects/rube-goldberg-machine/
type: Mechanical Design
description: We were tasked to create a Rube Goldberg machine to move a golf ball. This is my mechanism for the larger machine.
tags:
  - CAD
  - Engineering Design

repo_url: "#"
demo_url: "#"
image: /assets/images/SHAFT-ASSEMBLY (1).gif
placeholder: CAD render
---

## Overview

For my mechanical systems design class we were tasked with creating a Rube Goldberg machine which transports a gol ball. The requirements were to create a mechanism that moves the golf ball 1ft within 5 +/- 0.1 seconds while utilizing at least one linkage and one gear.
I chose a 'staircase' mechanism which uses oscillatory motion to translate the golf ball upwards and around a 90-degree turn. This was facilitated with a crankshaft and stepper motors. 

In addition to my own mechanism, I had the responsibility of timing and triggering my teammmates' mechanisms

This project was my introduction to microcontrollers and utilizing them to control electromechanical devices from sensor data.

## Showcase
<div class="project-inline-video">
    <iframe
        src="https://www.youtube.com/embed/XBgOeIWI5v4"
        title="Timing and Motor Control"
        loading="lazy"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        referrerpolicy="strict-origin-when-cross-origin"
        allowfullscreen>
    </iframe>
</div>

<div class="project-inline-video">
  <iframe
    src="https://www.youtube.com/embed/CzeYKJmA_Wk"
    title="Timing and Motor Control"
    loading="lazy"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
</div>
## Future Work

Despite the mechanism functioning, it is clear there is room for improvement. The alignment of parts caused catching, and the crankshaft was not balanced. This caused issues with torque resulting in jittery movement. If I were to do this project again, I would increase focus on part alignment and cooling of motor drivers to enable a higher current limit to increase motor torque.