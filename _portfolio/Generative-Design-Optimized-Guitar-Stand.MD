---
title: "Generative Design Optimized Guitar Stand"
excerpt: "Guitar stand designed in Fusion 360 and optimized using generative design for SLS manufacturing."
header:
  image: assets/img/physical_model.jpg
  teaser: assets/img/CAD.png
gallery:
  - url: /assets/img/physical_model.jpg
    image_path: assets/img/physical_model.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/full_view.jpg
    image_path: assets/img/full_view.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/front_view.jpg
    image_path: assets/img/front_view.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/side_view.jpg
    image_path: assets/img/side_view.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/side_view2.jpg
    image_path: assets/img/side_view2.jpg
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
  * The back of the stand (rectangular lip portion), which provides a connection point between the screw holes to the curved stand. The guitar itself serves as a large obstacle, obstructing the view of the curved stand from the screw holes; this allows for a clear connection point between the two.

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

It seems that generative design is very useful after several design iterations have been completed. Generative design should only be used when the engineer knows that their model fits the necessary size constraints. Since generative design studies take up a lot of time, to check if parts fit within certain models, the engineer should first design and fabricate simple shapes from CAD, and as those work, in later steps incorporate generative design. It is an extremely useful tool to functionally lightweight designs, as well as incorporate complex geometries that can be definitively supported by several fabrication methods that are declared in the study. Some limitations that may occur from utilizing generative design are that the engineer must definitively know where exactly each component falls in relation to the next, and exactly what loads the model might experience, and at what locations. Also, preserve geometries must be visible to each other; if obstacle geometries are blocking the view between two, the generative design study may falter in connecting those two components; this is something I initially struggled with, and thus had to add the back rectangular lip to the curved guitar mount so that the mounting screwholes could be efficiently connected. Generative design would be extremely useful in aerospace applications, where mass cuts are essential to ensure that systems can lift off without weight restrictions. However, for simple structural components like brackets of beams, generative design may add unnecessary time and complexity. 

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a47e7227ecb31351f4?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Forces Applied

| Force | Magnitude (lbf) | Location | Rationale |
|-------|-----------------|----------|-----------|
| Guitar Weight | 5 | Top Face of Guitar Mount | Vertical supported guitar weight on the mount. |
| Cable Weight | 1 | Top Face of Cable Mount | Vertical supported cable weight on the mount. | 
| Bearing Load on Screws | 52 | Inner cylindrical screwhole faces | Bearing load in the screwholes to mount the stand onto wooden wall. |
| Cable Removal | 15 | Cylinder sides of cable mount | Shear force on cable mount from cable removal. | 
| Guitar Removal | 8 | Sides of guitar mount | Shear force on guitar mount from rotating the guitar to remove from curved mount. |
| Swinging/Vibration | 4 | Right face of curved guitar mount | Lateral force from swinging/shaking guitar on mount. | 
| Swinging/Vibration | 4 | Left face of curved guitar mount | Lateral force from swinging/shaking guitar on mount. | 

![Iterations](/assets/img/iterations.png)
*Generative design iterations 10, 20, and 32 (final) of guitar stand, from left to right, respectively.*

![Rendering](/assets/img/rendering.png)
*Fusion 360 Rendering of guitar stand CAD model.*


{% include gallery caption="Physical Guitar Stand In Use" %}
