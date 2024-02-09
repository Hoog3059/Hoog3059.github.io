---
layout: post
title: Water rocket with data logger and parachute
description: A water rocket with an Arduino based flight computer, capable of logging flight data and deploying a parachute.
img: assets/projects/profielwerkstuk/thumbnail.jpg
date: 2021-01-15
importance: 20210115
category: personal
toc:
    sidebar: left
---

At the end of Dutch high school, you need to do a research project as preparation for university. A friend of mine and I built a water bottle rocket, with a built in, Arduino-based, flight computer, capable of logging flight data and deploying a parachute at the top of the trajectory.

Below I give a summary of everything that we have done. If you want all the details, please read our report (in Dutch) [here](/assets/projects/profielwerkstuk/verslag.pdf).

## Flight computer

The flight computer is tasked with logging flight data and deploying the parachute when at the top of the flight trajectory. The microprocessor at the heart of it al is an Arduino Nano. Acceleration is measured using an MPU6050. Barometric data is measured using a BMP280. All data is saved on a micro SD-card.

You can find the code of the flight computer here:
{% include repository/repo.liquid repository="Hoog3059/PWS_Boordcomputer" %}

<br>
{% include figure.liquid path="/assets/projects/profielwerkstuk/Boordcomputer_schematic.png" class="img-fluid rounded z-depth-1" style="color: white;" caption="Figure 1. Schematic of the flight computer. The bottom-left image is the same af the top-left, except with all components removed. The bottom-right image is the underside of the board." %}

<br>
{% include figure.liquid path="/assets/projects/profielwerkstuk/Boordcomputer_assembled.png" class="img-fluid rounded z-depth-1" style="color: white;" caption="Figure 2. Assembled version of the flight computer." %}

## Rocket assembly

<figure class="row">
  <picture class="col-sm-6">
    <img src="/assets/projects/profielwerkstuk/rocket.png" width="100%" height="auto" >
  </picture>
  <figcaption class="col-sm-6">
    Figure 3. Design of the rocket. The different elements are:<br>
    <ol>
        <li> PET-bottle as hull </li>
        <li> Duct tape </li>
        <li> Fins </li>
        <li> Flight computer </li>
        <li> Styrofoam nose cone </li>
        <li> Spring for deploying parachute </li>
        <li> Parachute rope </li>
        <li> Parachute </li>
        <li> Elastic band for opening parachute compartment </li>
        <li> Servo motor for parachute deployment </li>
        <li> Holder for flight computer </li>
        <li> Batteries </li>
        <li> Bottle connections </li>
        <li> Gardena nozzle </li>
    </ol>
 </figcaption>
</figure>

## Launch platform

<figure class="row">
  <picture class="col-sm-6">
    <img src="/assets/projects/profielwerkstuk/platform.png" width="100%" height="auto" >
  </picture>
  <figcaption class="col-sm-6">
    Figure 4. Design of the launch platform. The different elements are:<br>
    <ol>
        <li> Wooden stool </li>
        <li> Wooden sticks </li>
        <li> Rcoket </li>
        <li> Gardena female connector </li>
        <li> Garden hose </li>
        <li> Hose clamp </li>
        <li> Metal L-bracket </li>
        <li> Rope for disconnecting the Gardena connector, launching the rocket </li>
        <li> Metal ring </li>
    </ol>
 </figcaption>
</figure>

## Launch

Sadly, on the day of the launch, the parachute spring malfunctioned. You can watch the result in the video below.

{% include figure.liquid path="/assets/projects/profielwerkstuk/rocket_in_field.jpg" class="img-fluid rounded z-depth-1" style="color: white;" caption="Figure 5. The full rocket before launch." %}

<br>
<figure>
    <video preload="none" poster="/assets/projects/profielwerkstuk/rocket_flight_poster.png" style="width: 50%; margin-left: 25%;" controls>
        <source class="responsive-img-srcset" src="/assets/projects/profielwerkstuk/rocket_flight.mp4" type="video/mp4">
    </video>
    <figcaption class="caption">Launch of the rocket, with a crash at the end.</figcaption>
</figure>