---
title: "Bike Phone Holder; Top-Down Modeling Project"
excerpt: "Bike phone holder designed using top-down modeling approach, with no additional tools needed for implementation and snap orientations in landscape and portrait mode."
header:
  image: assets/img/complete_phone_mount.jpg
  teaser: assets/img/complete_phone_mount.jpg
gallery:
  - url: /assets/img/phone_mount_CAD.png
    image_path: assets/img/phone_mount_CAD.png
    alt: "placeholder image 1" 
  - url: /assets/img/phone_mount.jpg
    image_path: assets/img/phone_mount.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/detent_spinner.jpg
    image_path: assets/img/detent_spinner.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/detent_spinner_mount.jpg
    image_path: assets/img/detent_spinner_mount.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/detent_mechanism.jpg
    image_path: assets/img/detent_mechanism.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/clamp1.jpg
    image_path: assets/img/clamp1.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/clamp2.jpg
    image_path: assets/img/clamp2.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/pin.jpg
    image_path: assets/img/pin.jpg
    alt: "placeholder image 1" 
---

## Introduction: Top-Down Modeling

Top-down modeling refers to a methodology in which components are designed in reference to each other within one assembly. This allows for dimensions from components to be projected onto others, which lets any changes in one part automatically update other parts dependent on the original. Placing parts at their desired locations in relation to other parts also enables the use of as-built joints, which sets both components in place as they are built. Furthermore, this method eliminates the need to constantly go back and forth between separate models, as is traditionally required, since every single part of an assembly is defined as a new component within that assembly, instead of in a separate file. The top-down modeling method was utilized to design a bike phone mount that rigidly clamps onto bike handlebars, and allows for rigid mounting of a cell phone to sit within the mount and snap into both landscape and portrait orientations. 

## Design Rationale

This bike phone mount utilizes a detent mechanism to allow the phone to snap into landscape and portrait positions while on the mount. This mechanism consists of a compression spring, a ball bearing, and a spinner with four circular slots that the ball bearing will snap into due to the force that the spring imparts onto it. The detent mechanism mount includes a slot which encases the compression spring, and the detent spinner fits snugly within the mount, so that the ball bearing sits within half of the circular slot and half within the slotted portion of the detent mount above the compression spring. The compression spring has a 15 mm relaxed length, and the ball bearing has a diameter of 8 mm. The slotted portion is 18 mm in length, and the circular slot in the detent spinner has a radius of 4 mm. This gives the ball and spring 22 mm of space to fit in each of the four snap positions (90, 180, 270, and 360 degrees), and when compressed, gives the ball and spring 18 mm of space. Completely relaxed, the spring and ball would take up a total length of 23 mm. This length constraint provides adequate compression to allow for efficient rotation and snapping into position. 

The detent spinner mounts onto the handlebar clamp via a press-fit cylindrical extrusion, in which an extruded cylinder protruding from the clamp fits into a circular hole in the detent spinner. It was important during this design process to ensure that this fit was tight enough that it wouldn't fall off, but not too tight that the spinner could not spin, and also support the weight of the phone case spinning with it. It was also important to ensure that the detent spinner would press-fit onto the phone mount and prevent independent rotation of the phone mount with relation to the detent spinner. Because the phone mount was 3D printed from flexible TPU material, this tolerancing would be tighter than fitting into PLA. Thus, several design iterations were printed of the detent spinner, with varying circular hole dimensions (to fit onto the clamp and be able to rotate) and varying cylindrical extrusion diameter dimensions (for the phone mount to rigidly fit onto, so both would spin together). The final tolerancing between both PLA components (clamp and spinner) was 0.1 mm, and the tolerance between the spinner (PLA) and phone mount (TPU) was 0.002 mm. 

* The bike phone mount is comprised of the following 3D printed components: 
  * Handlebar Clamp 1 (PLA)
  * Handlebar Clamp 2 (PLA)
  * Detent Spinner Mount (PLA)
  * Detent Spinner (PLA)
  * Phone Mount (TPU)
  * Handlebar Attachment Pin (PLA)
* The phone mount was printed from TPU to serve as a flexible mounting mechanism that the phone could snugly fit into. The other aforementioned components were printed from PLA to serve as rigid, structural components. The bike phone mount also includes the following off-the-shelf components: 
  * Socket Head Screws
  * Heat Set Inserts
  * Stainless Steel Ball Bearing
  * Compression Spring 

## Assembly/Use Instructions
* Assembly Instructions
  * Insert M5 heat set insert into handlebar clamp 2. 
  * Insert handlebar attachment pin between handlebar clamps 1 and 2. 
  * Secure clamps around bike handlebar with M5 socket head screw and allen key. 
  * Insert M3 heat set inserts into handlebar clamp 1 for detent spinner mount to attach. 
  * Attach detent spinner mount to handlebar clamp 1 with M3 socket head screws and allen key.
  * Place compression spring and ball bearing into detent spinner mount slot. 
  * Attach detent spinner to handlebar clamp 1. 
  * Attach phone mount to detent spinner. 
  * Attach cell phone to phone mount.
* Use Instructions
  * Tilt cell phone in mount to landscape or portrait mode.
    * The ball bearing will snap the mount into place in each of these orientations. 
  * Attach/Remove cell phone as needed.

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



{% include gallery caption="Bike Phone Mount CAD Model, and Individual Components" %}
