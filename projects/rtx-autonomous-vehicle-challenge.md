---
layout: project
title: RTX Autonomous Vehicle Challenge
permalink: /projects/rtx-autonomous-vehicle-challenge/
type: Robotics
description: The 2026 RTX Autonomous Vehicle Challenge has teams build an unmanned ground vehicle and unmanned aerial vehicle to complete various tasks.
tags:
  - ROS 2

repo_url: "#"
demo_url: "#"
image: /assets/images/RTX_AVC.webp
placeholder: Robot screenshot
---

## Overview

The 2026 RTX AVC focused on a search and rescue mission containing one UAV and one UGV and consisted of 3 challenges. 
- Challenge 1 is a simple qualifier challenge where the UAV launches from the UGV, they both move in a straight line, 
then the UAV lands on the UGV. 
- Challenge 2 has the UAV launch from the UGV, scout a 15 x 15 yard field for an ArUco marker, communicate the location 
of this marker to the UGV, has the UGV drive to the marker while the UAV lands on the UGV. The challenge is complete when 
the UAV has successfully landed on the UGV and the pair are within 10 inches of the destination marker. 
- Challenge 3 is a repeat of challenge 2 with obstacles on the field.

After launching, there can only be direct communication between vehicles and no human guidance.

## Technical Information

The UGV was created from a goBILDA chassis, 2 Roboclaw 2x15A motor controllers, and 4 DC motors. We utilized an Nvidia 
Jetson Orin Nano Devlopment Kit as the main computer, and a ZED Mini Stereo Camera for Visual Inertial SLAM and state estimation.
ROS2 was used to communicate between sensors and electromechanical devices.


## My Role
Initially I started a UGV team member, working on wiring the motors and configuring the controllers to work with ROS2 on an 
Nvidia Jetson Orin Nano development kit. As time passed, I shifted towards assisting with integration testing between the UAV 
and UGV, with a focus on creating CAD.
I designed the UAV propeller guards, UAV/UGV ZED camera holder, UAV and UGV camera mount, UGV Landing Pad, and LiDAR holder. 
I wanted to focus on modular parts that could be removed if necessary for quick replacements or repositioning.

## Outcome
We were able to successfuly build a UAV and UGV that were capable of autonomous navigation. Unfortunately on competition 
day, a hardware failure caused the position estimate of the UAV to become unreliable, resulting in issues with the landing 
sequence and an incorrect destination ArUco marker location being sent to the UGV.

## Showcase
<div class="project-inline-video">
  <iframe
    src="https://www.youtube.com/embed/lQuj9eMAfHI"
    title="UGV Testing"
    loading="lazy"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
</div>

<div class="project-inline-video">
  <iframe
    src="https://www.youtube.com/embed/ogKHtgYL-0s?si=3N2SGP4JfujOvFFf"
    title="RTX Autonomous Vehicle Challenge video"
    loading="lazy"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
</div>