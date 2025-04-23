---
title: "Generative Design Optimized Guitar Stand"
excerpt: "Guitar stand designed in Fusion 360 and optimized using generative design for SLS manufacturing."
header:
  image: assets/img/CAD.png
  teaser: assets/img/CAD.png
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

## Discussion

Musicians need to store their instruments in safe and reliable ways, especially guitars. The stand must be rigid enough to support any loads that the instrument and the player impart onto it, and be optimized such that its mass is reduced while improving its mechanical performance. This project involved designing a guitar stand, optimizing its design for lightweightedness and structural support, and fabricating the model using SLS (Selective Laser Sintering). This model is designed to be screwed into wood, has a volume of about 25 cm^3, and has a mass of 25.7 g; this makes it easy to attach and remove to surfaces, light enough and small enough to be portable, for ease of travel. Most guitar stands support the guitar from the buttom: this offers support at the neck, offering an alternative small, lightweight, portable design. As a musician, I was interested in designing a model that would be useful for my own guitar, since I didn't own a stand, and it was a very fun project that I will now use!

## Preserve and Obstacle Geometry 

When designing the model, it was important to consider such regions as where the guitar was mounted on the stand, how it would be inserted, where the screwdriver to mount the stand would exist relative to the model, and others: these came to define the critical preserve regions and the obstacle geometry of the model. I started with the critical preserve regions.

![Preserve](/assets/img/preserve.png)
*Critical preserve regions of the guitar stand.*

* The critical preserve regions include the following: 
  * Two screw holes for #6 wood screws, with space for the screwhead, threads, and length. 
  * A mount to hang a 1/4" cable to plug the guitar in to an amplifier, with stoppers to prevent slipping and sufficient space for the width of multiple cable loops.
  * The curved stand portion, which supports the guitar between its head and neck. This has enough clearance for the guitar to be inserted diagonally, and it fits snug in place.
  * The back of the stand (rectangular lip portion), which provides a connection point between the screw holes to the curved stand. The guitar itself serves as a large obstacle (discussed later), obstructing the view of the curved stand from the screw holes; this allows for a clear connection point between the two.

The obstacle geometry in this model is defined by all the regions which relate to the guitar itself, tools to attach the stand to the wall, and the guitar cable.

![Obstacle](/assets/img/obstacle.png)
*Obstacle geometry of the guitar stand.*

* The obstacle geometry in this model includes the following:
  * The space taken up by the guitar cable as it is placed on the stand, and while it is supported by the stand.
  * The space taken up by the head, neck and base of the guitar as it is moved to be placed onto its mount, and as it sits on its mount.
  * The wall that the stand will be mounted on.
  * The screwdriver that will attach the screws into the screwholes and into the wall (2)

## Load Case Application and Structural Constraints

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a47e7227ecb31351f4?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>



{% include gallery caption="Bike Phone Mount CAD Model, and Individual Components" %}
