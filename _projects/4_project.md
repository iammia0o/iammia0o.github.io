---
layout: page
title: Hydist
description: Simulating Riverbank Erosion with GPU
img:  assets/img/hydist-cover.png
importance: 3
category: past work
---

Riverbank erosion poses a significant threat to the lives of thousands of people residing along the riverbanks. By accurately predicting the occurrence of erosion and understanding the impact of activities like sand mining on riverbanks, we can save countless lives. Riverbank erosion simulation can inform authorities to take prompt action and implement regulations to safeguard the riverbanks. However, simulating the impact of human activities on riverbanks requires extensive computational resources, hindering research progress.

In this project, we attempted to solve this computational bottleneck by building a simulation system on GPUs. Our system accurately simulated changes in river flow and riverbeds, providing information to predict riverbank erosion while running orders of magnitude faster than traditional simulation systems that run on CPUs. This project is a collaborative effort from researchers at UNIST, South Korea, and Vietnam National University, HCM.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/hydist_example.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A snapshot of our simulation result: Change in the riverbed from 1998 to 2002
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/scalability-hydist.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Scalibility of the model ran on GPU vs on CPU. 
 </div>


### Role: 
1. Collaborate with hydrologist scientist to create numerical solvers to Shallow-Water-Equations
2. Implement these solvers in python and validate the accuracy 
3. Implement these solvers in CUDA and validate the accuracy 
4. Optimize the performance of the CUDA code on NVIDIA Titan-X GPU

### Publication: 
Thi Kim, Tran, Nguyen Thi Mai Huong, Nguyen Dam Quoc Huy, Pham Anh Tai, Sumin Hong, Tran Minh Quan, Nguyen Thi Bay, Won-Ki Jeong, and Nguyen Ky Phung. 2020. "Assessment of the Impact of Sand Mining on Bottom Morphology in the Mekong River in An Giang Province, Vietnam, Using a Hydro-Morphological Model with GPU Computing" Water 12, no. 10: 2912. https://doi.org/10.3390/w12102912


### Patent: 
