---
title: "Microfluidic Device"
excerpt: "Microfluidic device for sorting particles by size ranging from 125 – 150 μm, and 425 – 500 μm."
header:
  teaser: /assets/img/microfluidic_device_path.png
gallery:
  - url: /assets/img/syringepumpgallery1.png
    image_path: assets/img/syringepumpgallery1.png
    alt: "placeholder image 1"
  - url: /assets/img/syringepumpgallery2.png
    image_path: assets/img/syringepumpgallery2.png
    alt: "placeholder image 2"
  - url: /assets/img/syringepumpgallery3.png
    image_path: assets/img/syringepumpgallery3.png
    alt: "placeholder image 3"
  - url: /assets/img/syringepumpgallery4.png
    image_path: assets/img/syringepumpgallery4.png
    alt: "placeholder image 4"
---

## Introduction 

Microfluidic devices manipulate small volumes of fluids, ranging from tens to hundreds of micrometers, within small channels. They are essentially like a circuit board for fluids, transporting them via small channels or tubes, to sort and mix reagants together. These devices allow for practical applications like lab-on-a-chip technology (scaling down multiple lab processes down to a single circuit or chip), multiplexing (multiple signal transmisssion from a single channel) and many others. To sort microfluidic particles by size, the pinch flow fractionation technique is utilized. After a liquid containing particles flows through a narrow channel, a second flow of liquid is introduced from the size, pinching this main flow into a narrow stream, and effectively forcing all particles to line up along one wall of the channel. When the pinched section ends, the particles start to spread out again; larger particles move farther away from the wall than smaller particles, creating distinct paths for differently sized particles. These particles are then collected separately by size via varying heights. To determine the particle position at a devices outlet, the following equation can be utilized: 

\[ Y_0 = \left(w_p - \frac{D}{2}\right) \frac{w_b}{w_p} \]

### Variables

- \( Y_0 \): The lateral position of the particle at the outlet.
- \( w_p \): The width of the pinched flow region.
- \( D \): The diameter of the particle.
- \( w_b \): The width of the main channel.

![Pinched Flow Diagram](/assets/img/pinched_flow_diagram.png)
*Pinched flow fractionation diagram and reference for particle position.*

A specific application requiring the sorting of small particles is the isolation of circulating tumor cells, or CTCs, from blood samples. CTCs are rare cells that shed from tumors and circulate in the bloodstream, and their isolation is critical to cancer diagnosis and treatment. Microfluidic devices offer a lower cost and effective method to isolate these cells based on their size differences. To do this, a blood sample is injected into the microfluidic device, and size-based sorting is completed via pinched flow fractionation. The sorted CTCs are then collected at specific outlets for further analysis (Sollier et al., 2014). 

## Instructions
* CAD Model Design:
  * Use Fusion 360 to design the microfluidic mold, adhering to the following specifications:
    * Device dimensions: 25 mm × 75 mm to fit on a standard microscope slide.
    * Channel dimensions: At least 1.2–1.5 times the diameter of the largest particle to avoid clogging.
    * Aspect ratio: Keep below 4:1 to prevent breakage during printing or demolding.
    * Inlets and outlets: Use 1.5 mm posts extruded above the mold for compatibility with microfluidic barbs.
    * Maintain symmetry in outlet channels; all outlet channel lengths should be equal to ensure consistent flow rates and prevent particle recombination.
    * Export the design as an STL file for 3D printing.
* Printing and Curing the Mold


• How to go from the 3D printed mold to the final device (Lab on a Chip paper). Include
the following steps but with additional detail:
o CAD model
o Print and cure mold
o Parylene device
o Cast PDMS
o Plasma bond glass slide
To go from 





{% include gallery caption="Syringe Pump Assembly Gallery" %}
