---
title: "MultiMaterial Pliers"
excerpt: "3D Printed, print-in-place functional pliers composed of PLA and TPU components."
header:
  image: assets/img/pliers.jpeg
  teaser: assets/img/pliers.jpeg
gallery:
  - url: /assets/img/pliers_cad.png
    image_path: assets/img/pliers_cad.png
    alt: "placeholder image 1" 
  - url: /assets/img/plier_components.jpg
    image_path: assets/img/plier_components.jpg
    alt: "placeholder image 1" 
  - url: /assets/img/pliers_closed.jpeg
    image_path: assets/img/pliers_closed.jpeg
    alt: "placeholder image 1" 
  - url: /assets/img/pliers.jpeg
    image_path: assets/img/pliers.jpeg
    alt: "placeholder image 1" 
---
## Project Description
This project involves designing and 3D printing functional needle nose pliers that can grip small components like through-hole resistors. The pliers are "print-in-place," meaning they are fully assembled right off the print bed, requiring no post-processing or manual assembly. Traditional print-in-place models require careful clearance gaps between moving parts; to reduce the "crunchy movement" of single material print-in-place designs occuring from plastic extrusion irregularities, these pliers utilize a multi-material assembly with flexible material (95A TPU) to achieve smooth movement, a spring-loaded return mechanism and improved functionality. 

Print-in-place parts are also widely used for fabricating mechanical toys and puzzles that include gears, hinges and interlocking mechanisms, like flexi-animals and interlocking puzzles. Print-in-place techniques are similar to advanced soft robotics fabrication methods, such as those demonstrated by university researchers [1] who utilized embedded 3D printing (EMB3D) to create pneumatic channels within elastomeric matrices for untethered soft robots. While their "octobot" required multi-step moulding and post-printing ink evacuation (not strict print-in-place), their research highlights how hybrid manufacturing can integrate rigid and flexible materials, which has been employed in this multimaterial pliers application. In terms of material combinations, rigid plastics like PLA, ABS or PETG work well for structural components when paired with flexible TPU for joints and springs.

## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a44a08e643800214da?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Design and Iterative Process
The MultiMaterial pliers are designed so that the flexible joint is made from 95A TPU to allow for continuous flexing, and the jaws and the handles are made up of rigid, PLA material. 

![Joint Jaw Design](/assets/img/jaws.png)
*Flexible Joint to Rigid PLA jaws.*

The design incorporates a diagonal triangular-like jaw design in the flexible component, that are angled so that the TPU bites into the rigid PLA and cannot fall out. There is 0.5 mm of clearance space between the flexible joint and the rigid handle/jaw, for ease of integration and to allow enough space for a press-fit, but not loose enough that the TPU joint can easily fall out. The pliers are approximately 300 mm tall, and approximately 140 mm wide, so that one's hand can easily and comfortably grip around the handles and squeeze accordingly. Fortunately, the first physical iterations of the rigid plier components and the joint were easily integrated, and functioned effectively.

* Plier Specifications:
  * Jaw Length: 70.6 mm 
    * The pliers can grip an object with a maximum depth of 70.6 mm. 
  * Jaw Capacity: 21.2 mm
    * The pliers can grip an object with a maximum width of 21.2 mm. 
## Print Settings
  * TPU Flexible Joint:
    * Infill Pattern: Rectinilear, 15%
    * Infill Width: 1 mm
    * Perimeters: 5
    * Horizontal Shells: 0 solid layers
  * PLA Rigid Components:
    * Infill Pattern: Gyroid, 25%
    * Infill Width: 0 mm
    * Perimeters: 2
    * Horizontal Shells: 4 solid layers

For the TPU flexible joints, a rectilinear pattern was chosen so that when the plier handles are squeezed, the grid-like structure bends cleanly along layer lines, and the stress is evenly distributed along those lines. A lower infill percentage was chosen to maximize bendability. The infill width of 1 mm ensures that each layer is stable while still maintaining bendability. 5 perimeters reinforce the joint's outer walls to resist tearing during repeated flexing. The absence of horizontal shells on the top and bottom of the TPU joint allows the joint to flex uniformly, as stiff shells would resist bending. The PLA rigid components were printed with the standard slicing parameters provided in the SuperSlicer software, as they are sufficient to maintain the pliers' durability. Please see below for images of the functional pliers picking up and placing down a resistor, and the pliers opening and closing.


![Functioning Pliers](/assets/img/pliers_r.gif)

![Pliers Squeeze](/assets/img/plier_s.gif)


## Citations

Wehner, M., Truby, R., Fitzgerald, D. et al. An integrated design and fabrication strategy for entirely soft, autonomous robots. Nature 536, 451–455 (2016). https://doi.org/10.1038/nature19100

{% include gallery caption="MultiMaterial Pliers CAD and Prototype" %}
