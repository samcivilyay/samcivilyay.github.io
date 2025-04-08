---
title: "Bike Phone Holder; Top-Down Modeling Project"
excerpt: "Bike phone holder designed using top-down modeling approach, with no additional tools needed for implementation and snap orientations in landscape and portrait mode."
header:
  image: assets/img/mount_physical_model.jpg
  teaser: assets/img/mount_CAD.jpg
gallery:
  - url: /assets/img/model_on_handlebars.jpg
    image_path: assets/img/model_on_handlebars.jpg
    alt: "placeholder image 1" 
---

## Introduction: Top-Down Modeling

A description of top-down modeling and how it was leveraged in this
assignment. 

## Design Rationale

• What type of rotation mechanism did you use? Does it work well?
• Did you have to change any dimensions to account for the 3D
printing process?
• What type of 3D printing did you use? Why?

## Assembly/Use Instructions

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4821cf8a08621cd53?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

figures:

▪ Real-life picture(s) of printed model in use on bike handlebars.
▪ Real-life .GIF of the holder rotating between landscape and portrait
▪ Fusion Rendering of phone holder with phone on it.
▪ Cross-section view of internal rotation mechanism. This can be a
screenshot of the design workspace with the section analysis tool.
CHBE 4200 Top-Down GitHub Project
▪ Individual images of each of the top-down components. This can be reallife or Fusion renderings.





![Pinched Flow Diagram](/assets/img/pinched_flow_diagram.png)
*Pinched flow fractionation diagram, equation, and reference for particle position.*


## Instructions
* CAD Model Design:
  * Use Fusion 360 to design the microfluidic mold, adhering to the following specifications:
    * Device dimensions: 25 mm × 75 mm to fit on a standard microscope slide.
    * Channel dimensions: At least 1.2–1.5 times the diameter of the largest particle to avoid clogging.
    * Aspect ratio: Keep below 4:1 to prevent breakage during printing or demolding.
    * Inlets and outlets: Use 1.5 mm posts extruded above the mold for compatibility with microfluidic barbs.
    * Use the particle position equation to determine the outlet heights of each differently sized particle. 
    * Maintain symmetry in outlet channels; all outlet channel lengths should be equal to ensure consistent flow rates and prevent particle recombination.
    * Export the design as an STL file for 3D printing.
* Printing and Curing the Mold
  * Resin Printing:
    * Slice the 3D model in PreForm for a Form 3+/4 printer with a layer thickness of 0.05 mm for high resolution. 
    * To avoid layer lines, ensure that the bottom of the mold is perfectly flat, and parallel to the resin vat. 
    * Post-Processing
      * Wash the printed mold for 5 minutes on the print bed in the FormWash, then remove it and wash for another 5 minutes in fresh IPA (isopropyl alcohol).
      * Dry the mold upside down for 30 minutes to prevent IPA pooling. Make sure that the inside of the mold has a homogenous sheen, and there are no glossy areas with uncured resin. Do not touch the inside of the mold
      * Gently blow off debris between the channels using compressed air, and then perform a 60 second surface cure with supports on to avoid warping.
      * Carefully remove support material without touching the inside of the mold.
    * Parylene Coating 
      * Place the mold in a parylene deposition machine.
      * Apply a thin, uniform layer of parylene-C to the mold.
    * Cast PDMS
      * Pour PDMS mixture into the parylene-coated mold, and degas to remove trapped air bubbles from channels.
      * Cure PDMS at 80 degrees C for 3 hours. 
    * Plasma Bond Glass Slide
      * Demold cured PDMS device carefully. 
      * Bond PDMS device to glass coverslip using a PlasmaFlo PDC-FMG plasma cleaner.


![Microfluidic Device Mold](/assets/img/ufluidic_mold.jpg)
*Microfluidic device resin printed mold.*

![PDMS](/assets/img/PDMS.jpg)
*PDMS casted microfluidic device.*



<iframe width="560" height="315" src="https://www.youtube.com/embed/2dfsqMubH2U" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>



{% include gallery caption="Microfluidic Device Physical Fabrication" %}
