---
layout: page
title: EMO-KNOW
description: Know your emotions
img: assets/img/emoknowcover.jpg
importance: 1
category: work
---

What make you feel what you feel?

Human emotions are complex and multifaceted. What make a person feel happy and delightful can make another person feel disappointed. The relationship between emotion cause and emotions is many-to-many. To augment AI a better understanding of the true nature of human’s emotions, a large dataset on emotion and emotion cause is needed. Existing datasets are small in scale; require extensive human labor to label emotions and emotions cause. Moreover, these labels are biased and subjective to the human labelers, and often limited to a few stereotypical emotions such as happy, sad, disgust etc; ignoring more nuanced emotions such as pride, gratitude, nostalgia, etc. 

EMO-KNOW is our effort to overcome these shortcomings of existing datasets. In this project, we curated a large scale dataset consisting of 9.8 millions tweets over 15 years of where users mentioned how they feel and what caused their feelings. 

In the first phase of the project, we created a dataset of 700,000 pairs of emotions and emotion causes, spanning 48 emotions.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/EMNLP_poster_5599.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Summaries of EMO-KNOW first phase, presented in EMNLP 2023
</div>


## Role:
1. Data curation : built scraping pipeline; explore data, refine search phrase
2. Data cleaning: applied different techniques to clean data:  remove hashtags, anonymize tweets. remove profanity, recover abbreviation, acronyms, etc
3. Data extraction: Created a finetuning dataset with GPT-3; tune different pre-trained LM for data extraction, evaluate them manually
4. Data validation: Design human validation metrics, run validation on Amazon Mechanical Turks
5. Paper writing
















<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>


You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %} -->
