---
layout: page
title: "PCBend: Light Up Your 3D Shapes With Foldable Circuit Boards"
author: "Marco Freire*, Manas Bhargava*, Camille Schreck, Pierre-Alexandre Hugron, Bernd Bickel, Sylvain Lefebvre (*Joint first authors)"
conference: "SIGGRAPH 2023"
teaser: "/assets/img/pcbend/teaser.png"
pdf: "/assets/pdf/pcbend/article.pdf"
---

**Marco Freire**\*<sup>1</sup>, **Manas Bhargava**\*<sup>2</sup>, Camille Schreck<sup>1</sup>, Pierre-Alexandre Hugron<sup>1</sup>, Bernd Bickel<sup>2</sup>, Sylvain Lefebvre<sup>1</sup>  
\*Joint first authors  
<sup>1</sup>Université de Lorraine, CNRS, Inria, LORIA, France  
<sup>2</sup>ISTA (Institute of Science and Technology Austria), Austria

[SIGGRAPH 2023](https://s2023.siggraph.org/), DOI: [10.1145/3592411](https://doi.org/10.1145/3592411)

![Teaser image](/assets/img/pcbend/teaser.png)

# Abstract
We propose a computational design approach for covering a surface with individually addressable RGB LEDs, effectively forming a low-resolution surface screen. To achieve a low-cost and scalable approach, we propose creating designs from flat PCB panels bent in-place along the surface of a 3D printed core. Working with standard rigid PCBs enables the use of established PCB manufacturing services, allowing the fabrication of designs with several hundred LEDs.

Our approach optimizes the PCB geometry for folding, and then jointly optimizes the LED packing, circuit and routing, solving a challenging layout problem under strict manufacturing requirements. Unlike paper, PCBs cannot bend beyond a certain point without breaking. Therefore, we introduce parametric cut patterns acting as hinges, designed to allow bending while remaining compact. To tackle the joint optimization of placement, circuit and routing, we propose a specialized algorithm that splits the global problem into one sub-problem per triangle, which is then individually solved.

Our technique generates PCB blueprints in a completely automated way. After being fabricated by a PCB manufacturing service, the boards are bent and glued by the user onto the 3D printed support. We demonstrate our technique on a range of physical models and virtual examples, creating intricate surface light patterns from hundreds of LEDs.


# Resources
- [Article]({{ site.baseurl }}{% link /assets/pdf/pcbend/article.pdf %})
- [Video](https://youtu.be/g8UX-KifGmM)
- [Code and data](https://github.com/mfremer/pcbend)
