---
layout: page
title: EMO-KNOW
description: Know your emotions
img: assets/img/emoknowcover.png
importance: 1
category: current work
---

What makes you feel what you feel?

Human emotions are complex and multifaceted. What makes one person feel happy and delighted can make another person feel disappointed. The relationship between emotion causes and emotions is many-to-many. To help AI understand the true nature of human emotions, a large dataset on emotions and their causes is needed. Existing datasets are small in scale and require extensive human labor to label emotions and their causes. Moreover, these labels are biased and subjective to the human labelers, and often limited to a few stereotypical emotions such as happy, sad, and disgust, ignoring more nuanced emotions such as pride, gratitude, and nostalgia.

EMO-KNOW is our effort to overcome these shortcomings of existing datasets. In this project, we curated a large-scale dataset consisting of 9.8 million tweets over 15 years, where users mentioned how they feel and what caused their feelings.

In the first phase of the project, we created a dataset of 700,000 pairs of emotions and emotion causes, spanning 48 emotions.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/EMNLP_poster_5599.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Summaries of EMO-KNOW first phase, presented in EMNLP 2023
</div>


### Role:
1. Data curation : Built scraping pipeline; explored data, refined search phrases.
2. Data cleaning: Applied different techniques to clean data: removed hashtags, anonymized tweets, removed profanity, recovered abbreviations and acronyms, etc.
3. Data Extraction: Created a fine-tuning dataset with GPT-3; tuned different pre-trained language models for data extraction, evaluated them manually.
4. Data Validation: Designed human validation metrics, ran validation on Amazon Mechanical Turk.
5. Paper writing



### Publication:
Mia Huong Nguyen, Yasith Samaradivakara, Prasanth Sasikumar, Chitralekha Gupta, and Suranga Nanayakkara. 2023. EMO-KNOW: A Large Scale Dataset on Emotion-Cause. In Findings of the Association for Computational Linguistics: EMNLP 2023, pages 11043–11051, Singapore. Association for Computational Linguistics.

{% raw %}
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
{% endraw %}
