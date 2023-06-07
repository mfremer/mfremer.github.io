---
layout: page
title: "PCBend: Light Up Your 3D Shapes With Foldable Circuit Boards"
author: "M. Freire*, M. Bhargava*, C. Schreck, P.-A. Hugron, B. Bickel, S. Lefebvre (*Joint first authors)"
conference: "SIGGRAPH 2023"
teaser: "/assets/img/pcbend/teaser.png"
image: "/assets/img/pcbend/reprimg.jpg"
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

# Citation
    @inproceedings{FreireAndBhargava2023PCBend,
      author = {Marco Freire and Manas Bhargava and Camille Schreck and Pierre-Alexandre Hugron and Bernd Bickel and Sylvain Lefebvre},
      title = {PCBend: Light Up Your 3D Shapes With Foldable Circuit Boards},
      journal = {ACM Transactions on Graphics (Proc. SIGGRAPH)},
      year = {2023},
      volume = {42},
      number = {}
    }

# Acknowledgements
We thank the reviewers for the valuable feedback. We also thank the Miba Machine Shop at ISTA, PCBWay, and PragoBoard for helping us with fabrication and assembly. This project was supported by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation program (Grant Agreement No. 715767 -– MATERIALIZABLE).

<img src="/assets/img/flag_eu.jpg" alt="EU flag" height="100"/>
<img src="/assets/img/logo_erc.jpg" alt="ERC logo" height="100"/>

# Resources
- [Article](https://manas-avi.github.io/publications/2023/PCBend/FoldableElectronics-2023-camera-ready.pdf)
- [Video](https://youtu.be/nJspqdpyWq4)
- [Code and data](https://github.com/mfremer/pcbend): coming soon!
