---
layout: project
title: Checkers Playing Gantry
permalink: /projects/checkers-playing-gantry/
type: Embedded Systems
description: Placeholder project for a controller board, actuator system, or firmware interface. Mention hardware constraints and how you validated the result.
tags:
  - Embedded C
  - Control

repo_url: "#"
demo_url: "#"
image: ""
placeholder: PCB / scope image
---

## Overview

This is a current work-in-progress project which aims to apply the topics I learned in MAE 6194 - Mechatronics. I aim to build robot that can play checkers and, in the future, chess. Currently, I have position control on a stepper motor
 and am in the process of fabricating the frame for the gantry.

## Technical Information
I am using TMC2209 stepper motor drivers and AS5600 magnetic position encoders for feedback motor control. Each Nema-17 Stepper motor will have its own Arduino nano running proportional control. These will be controlled by a main computer sending position commands via UART.