---
layout: post
title: Simple motion tracker
description: a project with a background image
img: assets/projects/eddy_current_brake/simple_motion_tracker.gif
date: 2022-04-20
importance: 20220420
category: personal
---

As part of <a href="/projects/university/eddy_current_brake/">this</a> university project, I needed to track a fiducial marker, in time, in a large set of slow-motion videos, and output the marker's position over time. Instead of doing this by hand using a tool such as <a href="https://physlets.org/tracker/">Tracker</a>, I decided to write a little tool that does it automatically.

The tool is written in Python and uses [OpenCV](https://opencv.org/) to do the tracking. The tool uses [template matching](https://docs.opencv.org/5.x/d4/dc6/tutorial_py_template_matching.html) to find the marker in each frame of a video.

<figure>
    <video preload="none" poster="/assets/projects/eddy_current_brake/eddy_current_brake_poster.png" style="width: 100%;" controls>
        <source class="responsive-img-srcset" src="/assets/projects/eddy_current_brake/eddy_current_brake.mp4" type="video/mp4">
    </video>

    <figcaption class="caption">Example of a fiducial marker being tracked. The green box indicates the searching area. The blue box indicates the found template. The red dot indicates the final logged position.</figcaption>
</figure>

The code can be found here:
{% include repository/repo.liquid repository="Hoog3059/template_tracker" style="width: 100%" %}