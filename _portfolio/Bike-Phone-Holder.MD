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

![Mount on Handlebars](/assets/img/mount_on_handlebars.png)
*Bike phone mount secured to bike handlebars.*

![Mount Rotating](/assets/img/mount_rotating.gif)
*Bike phone mount in use, rotating between landscape and portrait on handlebars.*

![Phone Holder with Phone](/assets/img/fusion_rendering.JPEG)
*Fusion rendering of phone holder with phone secured within.*

![Cross-Sectional View of Internal Rotation Mechanism](/assets/img/cross-sectional-view.png)
*Cross-sectional view of internal rotation mechanism within CAD model.*

{% include gallery caption="Bike Phone Mount CAD Model, and Individual Components" %}
