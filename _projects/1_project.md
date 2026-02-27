---
layout: page
title: ESFA
description: Efficiently large point FFT Acceleration on Versal ACAP architecture
img: assets/publication_preview/versal-tile2.png
importance: 1
category: 2025
related_publications: true
---


    ---
    Developed an accelerator on the Xilinx VCK190 platform to improve the throughput and efficiency of large-scale point FFT computations.
    ---

The fast fourier transform (FFT) is widely used to convert a time-domain signal into its frequency-domain representation in various fields. Previous works have demonstrated efficient FFT implementation on various accelerators. The emergence of AI Engines (AIE) on AMD Xilinx’s Versal ACAP brings the possibility of further improvement in computing efficiency. However, previous solutions have been restricted to a single-AIE manner, which limits the FFT size and neglects the potential of employing multiple AIEs. This paper proposes the ESFA framework, which can efficiently and automatically implement a scalable FFT on the Versal ACAP with multiple AIEs. The framework includes an analytical model to report the quality of results (QoRs) estimation for legal FFT partition modes, comprehensively covering the throughput-resource trade-off choices across the design space. In addition, the layout problem is formulated in an ILP to enhance the area efficiency. The framework also incorporates an automatic code generator to enable an agile implementation of the desired design. Our experiments on the VCK190 board show that we achieve 9,226/2,059 MS/s simulation/system throughput on the 1K-point FFT with a data width of 32, which obtains up to 10.1x speedup compared with AMD Xilinx’s library targeting AIE, meanwhile, 17.5x, 23.2x, and 0.9x speedup compared to the state-of-the-art designs on ASIC, CGRA, FPGA.

<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles. -->

