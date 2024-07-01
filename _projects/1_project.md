---
layout: page
title: EMO-KNOW
description: Know your emotions
img: assets/img/emoknowcover.png
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



## Publication:
Mia Huong Nguyen, Yasith Samaradivakara, Prasanth Sasikumar, Chitralekha Gupta, and Suranga Nanayakkara. 2023. EMO-KNOW: A Large Scale Dataset on Emotion-Cause. In Findings of the Association for Computational Linguistics: EMNLP 2023, pages 11043–11051, Singapore. Association for Computational Linguistics.

```bibtex
@inproceedings{emo-know-huongnguyen-2023,
    title = "{EMO}-{KNOW}: A Large Scale Dataset on Emotion-Cause",
    author = "Nguyen, Mia Huong  and
      Samaradivakara, Yasith  and
      Sasikumar, Prasanth  and
      Gupta, Chitralekha  and
      Nanayakkara, Suranga",
    booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2023",
    month = dec,
    year = "2023",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.findings-emnlp.737",
    doi = "10.18653/v1/2023.findings-emnlp.737",
}
```

