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

After defining the obstacle and preserve geometries, it was important to consider regions that would be taken up by the player placing the guitar in the stand, the cable hanging on its stand, and what loads would be imparted onto the model by either the player, the guitar, or the cable. Firstly, a fixed structural constraint was placed on the inner cylindrical face of both screwholes, since the mount is designed to be screwed into the wall, and does not move. This ensures that the location and the shape of this region remains the same throughout the generative design study. Following this step, the forces that both the guitar, the player, and the cable would impart onto the stand were determined and incorporated into the study. 

![Loads](/assets/img/loads.png)
*Structural loads applied to the guitar stand.*

* The following loads were applied to the model: 
  1. 5 lbs applied to the top face of the curved mount. This represents the weight of the guitar that is supported by the mount. This was determined by physically weighing the guitar, applying a safety factor of 1.25 and understanding that its weight is applied vertically down on the stand as it is supported.
  2. 1 lb applied vertically downward onto the guitar cable mount. This represents the weight of the cable supported by the mount, and was determined by weighing the cable itself and applying a safety factor of 2.
  3. 52 lbs applied as a bearing load to both screwholes. Plywood (to screw the mount into) has a bearing strength of approximately 500 psi, and the screwholes are designed for #6 wood screws. The screw diameter is 0.138", and is about 0.75" embedded into the wood. Thus, the projeted bearing area is 0.104 square inches. The bearing load is 500 psi * 0.104 in^2 = 52 lbs. 
  4. 15 lbs applied along the sides of the cylindrical cable mount, representing the shear force on the mount from yanking the cable sideways to remove it. 15 lbs was used as a conservative estimate in case the player applied an aggressive pull on the cable.
  5. 8 lbs applied along the sides of the guitar mount perimeter, representing the shear force on the mount when turning the neck of the guitar so it can come out of the stand. 8 lbs was used as a conservative estimate in case the player aggressively and rapidly turned the guitar against the mount. 
  6. 4 lbs applied to the right face of the curved guitar mount. This represents the lateral force onto the right face that might come from the guitar swinging back and forth or shaking on the mount. 4 lbs is the weight of the guitar.
  7. 4 lbs applied to the left face of the curved guitar mount. This represents the lateral force onto the left face that might come from the guitar swinging back and forth or shaking on the mount. 4 lbs is the weight of the guitar.

* To further refine the loads, the real-world prototype could be rigidly attached to a wall, and the following load tests could be done:
  * Placing the guitar within its mount and shaking it vigorously side to side.
  * Swinging the guitar back and forth on the mount.
  * Sliding the guitar along the walls of the curved portion.
  * Sliding the cable back and forth along its mount.
  * Applying vertical pressure to the top of the cable as it sits on its mount. 
* If any of these tests fail, the loads could be increased in the generative design study, and new loads could be added as visualized from testing.

## Critique of Generative Design

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a47e7227ecb31351f4?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>



{% include gallery caption="Bike Phone Mount CAD Model, and Individual Components" %}
