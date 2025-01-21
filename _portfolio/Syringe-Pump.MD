---
title: "Syringe Pump"
excerpt: "DIY syringe pump capable of 1 uL / min flow rate up to 10 mL / min"
header:
  image: /assets/img/syringepumpcover.png
  teaser: /assets/img/syringepumpteaser.png
gallery:
  - image_path: assets/img/syringepumpgallery1.png
  - image_path: assets/img/syringepumpgallery2.png
  - image_path: assets/img/syringepumpgallery3.png
  - image_path: assets/img/syringepumpgallery4.png
---

# Project Details/Features 

The purpose of this project was to design and build a cost-effective, highly accurate syringe pump as an alternative to expensive commercial models. The key features of the design include:
* Precise liquid dispensing using a stepper motor and lead screw mechanism
* Multi-directional pump feature for filling and expelling liquids
* Compatibility with different syringe sizes (20 mL and 10 mL)
* LED indicator for operational status (green for running, yellow for paused, red for stopped)
* Modular design for effective disassembly and recycling of 3D-printed components
* Parameterized CAD design for easy modifications

# Off-The-Shelf Parts 

| Part | Description |
|------|-------------|
| Stepper Motor | [NEMA 17 with 1.8-degree angle (200 steps/revolution)](https://www.amazon.com/gp/product/B07LF898KN/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&th=1) |
| Lead Screw | [2 mm lead](https://www.amazon.com/dp/B07R1H5ZMV/ref=cm_sw_em_r_mt_dp_0YZ13D4HQBGW2Z86PBV1?_encoding=UTF8&psc=1) |
| Lead Screw | [8 mm lead](https://www.amazon.com/gp/product/B0B8RKN89V?ie=UTF8&th=1&linkCode=sl1&tag=drd0cf-20&linkId=bb4eefbbfff880704d7cd0784b1af8c0&language=en_US&ref_=as_li_ss_tl) |
| Flexible Coupler | [1/4th inch by 8 mm coupler](https://us.openbuilds.com/1-4-x-8mm-flexible-coupling/) |
| Linear Rod | [200 mm length with 8 mm diameter](https://www.amazon.com/dp/B07MPGWJMS/ref=cm_sw_em_r_mt_dp_X5AQS0ES7JH8JG83AAZ3) |
| Linear Bearing | [For 8 mm diameter rod](https://www.amazon.com/gp/product/B087WPGQ8T/ref=ppx_yo_dt_b_asin_image_o00_s00?ie=UTF8&psc=1) |
| Aluminum Extrusion Bar | [1 inch length for mounting components](https://us.openbuilds.com/v-slot-20x40-linear-rail/) |
| Power Supply | [MEAN WELL RQ-65D AC-DC Power Supply Quad Output 5V 12V 24V 12V 4 Amp](https://www.amazon.com/dp/B005T9HGLI/ref=cm_sw_em_r_mt_dp_A8CZ056TM52EJGZTGZGR?_encoding=UTF8&psc=1) | 
| Microcontroller | [Arduino Uno](https://www.amazon.com/dp/B007R9TUJE/ref=cm_sw_em_r_mt_dp_TY8JGK0CJD1JEJM4BNNJ) | 
| A4988 Stepper Driver | [To control stepper motor movement](https://www.amazon.com/dp/B01FFGAKK8/ref=cm_sw_em_r_mt_dp_V0YKTYKDWMR8WHTKA53T?_encoding=UTF8&psc=1) |
| Breadboard | [For circuit connections](https://www.amazon.com/dp/B082VYXDF1/ref=cm_sw_em_r_mt_dp_N6Q28CAGPAYCKCSJKDDC?_encoding=UTF8&psc=1) |
| Push Buttons | [One latching, two non-latching](https://www.amazon.com/dp/B07XTBL1NP?psc=1&smid=A2NNH5C5IP9N3O&linkCode=sl1&tag=drd0cf-20&linkId=43b42a7cb2a088ebd85d65cb9da46725&language=en_US&ref_=as_li_ss_tl) |
| Limit Switch | [For stopping the motor when syringe is empty](https://www.amazon.com/gp/product/B073TYWX86/ref=ppx_yo_dt_b_asin_image_o01_s00?ie=UTF8&psc=1) |
| LED | [Multicolored](https://www.amazon.com/dp/B0194Y6MW2/ref=cm_sw_em_r_mt_dp_FW3CFQT7ZGFQ2R04N6G3?_encoding=UTF8&psc=1) |

# Arduino Code

*[Syringe Pump Code](https://github.com/samcivilyay/Syringe_Pump_Project_SC/blob/main/Syringe_Pump_Arduino_Code)



