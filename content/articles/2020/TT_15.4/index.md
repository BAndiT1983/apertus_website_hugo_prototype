---
title: AXIOM Team Talk 15.4 - Optical Filters & Firmware 2.0
date: 2020-03-17T18:50:00+02:00
author: Sebastian
teaser_image: images/Team-Talk154-Title-sq.jpg
---

This is part four of a recently shot round of AXIOM Team Talks. For the previous episodes please see AXIOM Team Talk archive. 

<!--more-->

## Optical Filters: Ultraviolet/Infrared Cut Off in the AXIOM Beta

We humans see colours because of light’s having different wavelengths. The part of the electromagnetic spectrum that’s visible to the human eye measures from around 400 nanometers (nm) to around 700 nm with what non-colourblind people perceive as colours ranging from blue, running through the various colours of the rainbow and ending at red. The area that’s slightly outside human vision’s perceptibility at the low end is called ultraviolet and at the high end infrared light. Image sensors like the CMV12000 in the AXIOM Beta capture a wider spectrum of light wavelength than our eyes can see.
Light Spectrum

## CMV12000 Response Curve

To eliminate so-called Infrared (IR) pollution, cameras traditionally utilise a reflective filter, often glued directly to the image sensor surface, which prevents the undesired wavelengths from passing through to the image sensor. In the AXIOM Beta Compact enclosure everything is intended to be flexible depending on the camera’s use-case, so it was appropriate for the UV/IR filter to be modular in its installation. The optical path of the AXIOM Beta Compact features two optical filter holder slots; one to be filled with the UV/IR filter and the second left empty for future any additions or so as to leave space for creative choice filters. This means it’s possible to remove filters if capturing the full spectrum available to the image sensor is required.
Optical Filter

AXIOM Beta Compact Optical Filter Holder
AXIOM Beta Compact Optical Filter Holder - Second generation prototype - note the newly added rubber sealing.

The Flange-Focal-Distance (FFD), which is the measurable distance between the image sensor surface and lens bayonet, has to compensate for the width of any glass elements that are introduced into the optical path of the sensor. If not then the focus plane will be off (meaning the lens markings for the focus distance will not be correct and, in a worst case scenario, getting an image precisely in focus will be impossible). To address this the optical filter holders have an accurately produced thickness which exactly matches the FFD compensation of the optical filter in the holder.
AXIOM Beta Compact Optical Path

We have sourced samples from several filter manufacturers and not only measured them with a scientific spectrometer - surprise surprise: in tests, some of the filters demonstrated marked discrepancies against the wavelength specifications provided by manufacturers - but also captured test-shots with the AXIOM Beta. Below you can view/download a few of those shots:

Download all captured raw12 files
Here is the documentation about the DNG conversion, note that these images have no FPN or black calirabtion files available.
Without UV/IR filter
Without UV/IR filter (note that the error columns on the right are due to a connectivity issue with some image sensor lanes in this particular prototype camera).
With the Bohr Optics UV/IR filter
With the Bohr Optics UV/IR filter (note that the error columns on the right are due to a connectivity issue with some image sensor lanes in this particular prototype camera)

## AXIOM Beta Firmware 2.0 - Continuous Integration

The AXIOM Beta runs Linux as its onboard operating system via two ARM cores, so what we call ‘Firmware’ is basically the complete underlying system image with all its drivers, tools, binaries, scripts and utilities. The colleagues behind the AXIOM Micro have set up a continuous integration system that pulls all sources for said tools, drivers, etc. and assemble a complete, new firmware image automatically and periodically. This way any changes and improvements that might be made to any aspect of the camera's software, at any time, are made immediately available to all users in nightly/unstable firmware releases. The term “unstable” refers to the fact that the automatically generated firmware images are not tested by humans on the actual camera hardware prior to release - so, like with updates to an operating system on a laptop, something might not initially work as expected. Similarly, stable development releases that are verified on the actual hardware will ultimately be made available for download periodically in the future. This new firmware is called "Firmware 2.0" and due to the ongoing restructuring, new documentation is required (tools/scripts are in different folders or have a slightly different name, etc.). Updating the camera’s firmware documentation to correspond with improvements is underway on the wiki but any additional help with reviewing, improving and extending it would be appreciated as always.
Telegram

Development updates are frequently posted inside the project's Telegram group as it's easier and faster than via newsletters or articles such as this. Salient points from meeting notes are typically posted there most Mondays too. If you'd like to keep an eye on general developments as they happen and get involved with discussion or ask questions, then please feel free to join.
Further Links

    Newsletter editions - Previous, HTML newsletters archived. Subscribe here to receive yours via email.
    Shop links, prices and availability
    Camera structure - A complete guide to the camera's specifications and components.
    AXIOM Beta sample videos - Uncompressed .mov .mp4 and .dng files in 720p, 1080p and 4K are archived here if you'd like to play with them.
    Pre-order notification - Receive an email when a more user-friendly version of the camera is ready to ship.
    GitHub Repository
    Join the Team
    Social accounts - Links to YouTube etc.
    AXIOM Project Background - How apertus° and the AXIOM project got started.


Want to participate?

Want to provide feedback or suggest improvements? Want to try your own approach and need help?

Get in touch via IRC or email.
Project: 
AXIOM Beta