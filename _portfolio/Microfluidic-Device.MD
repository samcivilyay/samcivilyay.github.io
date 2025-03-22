---
title: "Microfluidic Device"
excerpt: "Microfluidic device for sorting particles by size ranging from 125 – 150 μm, and 425 – 500 μm."
header:
  teaser: /assets/img/microfluidic_device_path.png
---

## Introduction 

Microfluidic devices manipulate small volumes of fluids, ranging from tens to hundreds of micrometers, within small channels. They are essentially like a circuit board for fluids, transporting them via small channels or tubes, to sort and mix reagants together. These devices allow for practical applications like lab-on-a-chip technology (scaling down multiple lab processes down to a single circuit or chip), multiplexing (multiple signal transmisssion from a single channel) and many others. To sort microfluidic particles by size, the pinch flow fractionation technique is utilized. After a liquid containing particles flows through a narrow channel, a second flow of liquid is introduced from the size, pinching this main flow into a narrow stream, and effectively forcing all particles to line up along one wall of the channel. When the pinched section ends, the particles start to spread out again; larger particles move farther away from the wall than smaller particles, creating distinct paths for differently sized particles. These particles are then collected separately by size via varying heights. To determine the particle position at a devices outlet, the following equation can be utilized: 

![Pinched Flow Diagram](/assets/img/pinched_flow_diagram.png)
*Pinched flow fractionation diagram, equation, and reference for particle position.*

A specific application requiring the sorting of small particles is the isolation of circulating tumor cells, or CTCs, from blood samples. CTCs are rare cells that shed from tumors and circulate in the bloodstream, and their isolation is critical to cancer diagnosis and treatment. Microfluidic devices offer a lower cost and effective method to isolate these cells based on their size differences. To do this, a blood sample is injected into the microfluidic device, and size-based sorting is completed via pinched flow fractionation. The sorted CTCs are then collected at specific outlets for further analysis (Sollier et al., 2014). 

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

## Discussion
Resin printed molds often contain uncured resin residues on their surfaces, even after post-processing. These residues can inhibit the curing of PDMS, which leads to incomplete crosslinking and a sticky, non-functional device. Parylene acts as a barrier layer, which prevents uncured resin from interfering with the PDMS curing process. Parylene coating also creates a smooth and uniform surface ideal for replicating fine microfluidic features in PDMS. The microfluidic sorting device created can be used for a variety of applications, including: 
  * Sorting red blood cells, white blood cells and platelets for diagnostic purposes.
  * Sorting microplastics by size to study their distribution and environmental impact in water samples.
  * Sorting bacteria or yeast for quality control in food and beverage production.

![Microfluidic Device Mold](/assets/img/ufluidic_mold.jpg)
*Microfluidic device resin printed mold.*

![PDMS](/assets/img/PDMS.jpg)
*PDMS casted microfluidic device.*

My design incorporates an inlet/outlet channel width of 0.75 mm, which is 1.5 times greater than the largest particle size of 500 micrometers, preventing particles from getting stuck or blocked as they travel, and ensuring laminar, and even flow distribution. The pinched section width is 0.5 mm, which is 1.25 times the largest particle size; the narrower width increases fluid velocity in the pinched region and forces particles in a line along the wall, but is still large enough to prevent any clogging. The broad section encompasses the entire height of the microfluidic device to allow for efficient particle separation. There are three outlet ports. The highest outlet port is for particles sized between 125-150 micrometers, and thus includes heights between 16.15 mm and 16.625 mm, as calculated from the particle position equation. The middle outlet port is for particles sized between 425 and 500 micrometers, and thus includes heights between 9.5 mm and 10.925 mm, as calculated. The lowest outlet port collects any larger particles that fall below 6 mm. The outlet channels are all the same length, approximately 20 mm, to ensure consistent flow rates. Corners in the model are rounded to prevent any disruptions to streamlines and maintain proper separation. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/2dfsqMubH2U" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

As shown by the testing video here, the larger, purple particles tended to separate downwards from the smaller, orange particles. However, at times, the larger particles still exited from the taller outlet. This indicates that perhaps the entrances to each outlet channel should have been more compressed, so that particles at certain heights were encouraged to exit as closest to their location as possible, through the correct outlet. Additionally, at times, particles bumped into each other, and because of this, exited through the incorrect outlet. To further optimize the design, in the future, outlet channels could be more staggered to minimize overlap, and perhaps baffles could be added near outlet entrances to help better guide particles into the correct channel.  

## Citations

Sollier, E., Go, D. E., Che, J., Gossett, D. R., O'Byrne, S., Weaver, W. M., ... & Di Carlo, D. (2014). Size-selective collection of circulating tumor cells using Vortex technology. Lab on a Chip, 14(1), 63-77. DOI: 10.1039/C3LC50689D
