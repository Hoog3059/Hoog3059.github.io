---
layout: post
title: Eddy currents braking force
description: Validating a model for the braking force due to eddy currents.
img: assets/projects/eddy_current_brake/field_density.png
date: 2022-04-20
importance: 20220420
category: university
related_publications: true
---

*By Neil Eshuis, Timo Hoogenbosch and Remi van den Berg.*

A fundamental flaw in traditional braking systems is that they are prone to wear due to friction. Eddy current brakes are an alternative braking system in which the kinetic energy of the object is dissipated by an electric current induced in a conductor by a magnetic field, eliminating the need of friction thus reducing the wear on the brakes. This experiment aims to validate a model proposed by {% cite eddyCurrentBrake_ModelByHeald %} in regards to the relation between the braking force due to eddy currents and the magnetic field strength, as well as the relative velocity between the magnetic field and the conductor. This was done by repeatedly firing a cart supporting two magnets mounted on a C-channel along an air track whilst varying the magnetic field strength by increasing the magnet-to-magnet distance. An aluminium bar functioning as the conductor was suspended inside the C-channel whilst a high speed camera was used to film the runs. [Custom tracking software](/projects/personal/simple_motion_tracker) was used to track the location of the cart along the track and to allow the data to be analysed. The cart is illustrated by Figure 1 and 2, and the measurement setup is illustrated by Figure 3.

To validate the model, the measured cart trajectory and force-velocity relation were compared to those predicted by the model, by using them to determine the magnetic field strength between the magnets. The field strength determined using the trajectory differed by ($$ 1.3\pm0.4 $$ )% and the field strength determined using the force-velocity relation differed by ( $$ 1.7\pm0.8 $$ )%. Since these are both lower than 5% it is concluded that the model is validated for the used measurement setup.

You can read the full research report [here](/assets/projects/eddy_current_brake/report.pdf). You can find all data, and the data processing code [here](https://deepnote.com/@Eindproject-Inleidend-Practicum/Eindproject-4c837f89-d637-46c5-96f6-75f46b71cb05).

<div class="row justify-content-sm-center">
    <div class="col-sm-6">
        {% include figure.liquid path="/assets/projects/eddy_current_brake/kar.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
        Figure 1. The cart used on the air track. A lego structure is used to make a trough through which an aluminium bar can pass. On each side of the trough is space for magnets.
    </div>
    <div class="col-sm-6">
        {% include figure.liquid path="/assets/projects/eddy_current_brake/kanaal.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
        Figure 2. An aluminium bar passing through the trough attached to the cart.
    </div>
</div>
<br>
<div class="row justify-content-sm-center">
    <div class="col-sm-8">
        {% include figure.liquid path="/assets/projects/eddy_current_brake/setup_side_view.png" title="example image" class="img-fluid rounded z-depth-1" %}
        Figure 3. Illustration of the measurement setup, side view. 1: Air pump, 2: Magnetic launcher with rubber band, 3: Magnets on C-channel, 4: Air track cart, 5: Air track, 6: Conductive plate, 7: Stand (with a clamp to hold the conductive plate in yellow).
    </div>
</div>
<br>
