---
title: Design Intervention Summary
excerpt: ""
header:
    overlay_image: /assets/images/design-banner.png
toc: true
toc_label: "Table of Contents"
#toc_icon: "cog"
gallery:
  - url: /assets/images/feather-huzzah32.png
    image_path: /assets/images/feather-huzzah32.png
    alt: "Adafruit Feather HUZZAH32"
    title: "Adafruit Feather HUZZAH32"
  - url: /assets/images/feather-footprint.png
    image_path: /assets/images/feather-footprint.png
    alt: "Adafruit Feather Footprint"
    title: "Adafruit Feather Footprint"
---

The result of this research is a proposal for an immersive designs system called PAINT!, or Prototype and install, no trouble! The proposal is not meant to be the final design concept, but a set of design pillars that the features of the toolset should support (or at least not hinder), along with design choices that I believe would be ideal if the resources were available to develop the toolset now. These are the four design pillars:

**A Network of Things:** All devices should have modern wireless communications as a given, which has become cost-effective in just the last few years.

**Accessible Iteration:** The tools should strive to close the gap between when creative design and prototyping with technology. Usually live-action game designs are completed before the technology is tested. Creative design should occur with technology, not for it.

**Open and Off-the-shelf Support:** Technology and standards can change quickly! Care must be taken in how the tools are designed and what standards are used or created to ensure they support wide accessibility for designers, not necessarily the latest and greatest features, especially if that limits who can use them.

**Prototype Permanence Path:** Taking a project from design concept to having it installed and ready for an audience is hard work! The toolset should help designers move through the phases of their project and result in dependable, maintainable work.

## Paint! Flow - Design Software
_Flow_ is the software side of the toolset. It is proposed to use Node-RED, an existing open-source codeless logic solution, as the starting codebase. The node based logical structure reduces the barrier for designers, not requiring software coding in order to create logic. As a visual language, it can also serve as a strong tool for communicating design flow to the rest of the design team.

[//]: # (![full]({{ site.baseurl }}/assets/images/node-red-example.png){: .full})

{% include figure image_path="/assets/images/node-red-example.png" alt="Example Node-RED Flow" caption="_An example logic flow for reacting to the success or failure of a keypad code._" %}

This software will not only serve as the tool for designing the logic in a live-action game but also allow for monitoring the game as it runs.

## Paint! Palette - Microcontroller Shield
Each device involved in running aspects of the live-action game are on a network that _Flow_ will manage. The _Paint! Palette_ is a microcontroller shield that will support the growing library of Feather compatible microcontroller boards, initially developed by Adafruit. This new standard will leave room for growth as new boards that support the [Feather specification](https://learn.adafruit.com/adafruit-feather/feather-specification) will either be immediately compatible or can be added with little effort.

{% include gallery caption="_Left: The Adafruit Feather HUZZAH32. Right: The Feather footprint specification._" %}

The _Palette_ is also meant to help designers from the early design phases of their live-action game through to installation and support. It will provide a combination of standard connections for LEDs, [Sparkfun’s Qwiic system](https://www.sparkfun.com/qwiic) for communicating with I2C sensors, and the ability to wire directing to the board with prototyping wire, or more permanently with screw terminals. The board will also be designed for easily mounting for when it comes time to install.

## Project Phases
Many of the planned _PAINT! Palette_ features are meant to provide ease of use on the front end and reliability on the back. Attention is being paid to methods of wiring, power routing and regulation to support a large variety of electronics, easy methods for adding or altering devices, and more to support the path from prototyping to permanence. This also extends to the software that will run on the _Palettes_ and _Flow_.

Security, for instance, is a feature that should evolve throughout a project. During early stages of design security is often more of a hindrance than help. At this stage, setting up new devices and networks should be fast and easy, not resistant to change. As development continues, security is useful for preventing accidental changes and reducing access, until installation, where change should be highly restricted. You don’t want visitors to your live-action game messing around on your wireless network!