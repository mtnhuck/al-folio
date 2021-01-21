---
layout: page
title: Mental Health
description: depression, anxiety and brain connectivity
img: /assets/img/mental_health3.png
---
[Integrating Smartphone Sensing, Surveys and MRI Data: Proof of Concept](https://www.frontiersin.org/articles/10.3389/fnins.2019.00248/full)

Almost 1/3 of college students have clinically relevant levels of affective disorders, such as anxiety or depression. Understanding factors that predispose individuals to these disorders or trigger their onset may allow for improved secondary educational institutional interventions which could beneficially impact upwards of 5 million individuals (18.4 million college students in in the US <a href="census.gov”>in the latest census</a> ], assuming 30% occurrence of either depression or anxiety).

Through mobile sensing (StudentLife app: https://studentlife.cs.dartmouth.edu/) we can collect data from individuals’ smartphones in a more ecologically valid manner than available in traditional lab settings. Paired with with real-time surveys, termed EMA’s (Ecological Momentary Assessments), we are able to pair passive smartphone measurements with  self-reported surveys. Individuals in these studies participate in functional MRI sessions and return year-after-year throughout their college experience. In a proof-of-concept study to combine these diverse modalities we correlated brain connectivity with phone usage. Connectivity between the subgenual cingulate cortex (sgCC) the duration of phone usage with resting-state functional connectivity from the subgenual cingulate cortex. We observed a negative relationship with sgCC-OFC connectivity and a variety of phone usage and depression metrics.

<img class="col three left" src="{{ site.baseurl }}/assets/img/StudentLifeStudyFlow.png" alt="" title="Figure 1"/>

<img class="col three left" src="{{ site.baseurl }}/assets/img/PhoneUsage_sgCC.png" alt="" title="Figure 1"/>

<div class="col three caption">
    Top: Study workflow.
    Bottom: Exploratory analysis correlation sgCC RSFC seedmaps correlated with mean unlock duration identified a cluster with a positive relationship to unlock duration in the ventromedial prefrontal cortex (p < 0.01, volume corrected using ACF to p < 0.001) shown on inflated lateral (top left), medial (bottom left) and ventral (right) cortical surfaces. The sgCC seed is represented as a black 10 mm sphere, larger than the 4 mm sphere used to create the seedmaps for visualization purposes.
</div>

Across both cohorts, the more individuals used their phone, the less connectivity was observed between sgCC and OFC. Similar patterns were observed for self-reported depressive symptoms and circadian rhythm consistency. These results are correlational and should be interpreted with caution. Our primary motivation for publishing this article was to show that, even with relatively rudimentary analyses, links between self-reported mood score, passive mobile smartphone sensing and functional brain imaging can be observed.


[Causal Relationships Between Mental Health Metrics](https://doi.org/10.2196/16684)


The above mentioned analyses provide insight into correlations between brain connectivity, phone usage and mood, but do not provide insight into causality. To begin to identify causal, or temporally lagged relationships over time, we applied Peter and Clark Momentary Conditional Independence (PCMCI) to mental health metrics such as depression, anxiety, stress and self-esteem. We were able to identify causal and contemporaneous relationships between these mental health metrics and replicate them across the first year of college of two distinct cohorts.

<img class="col three left" src="https://asset.jmir.pub/assets/f8b842ca8c158bf781e7bb39eb3a466c.png" alt="" title="Figure 1"/>

<div class="col three caption">
    Causality graph observing previous week (t-1) connections on mental health metrics collected through ecological momentary assessments weekly for cohorts 1 (top left) and 2 (top right). Contemporaneous connections presented for cohorts 1 (bottom left) and 2 (bottom right). Solid lines are positive relationships and dashed lines are negative relationships with magnitude marked on the graph, listing the partial correlation value. For causal relationships, the arrowhead signifies directionality. Anx: anxiety; Dep: depression; SE: self-esteem; Str: stress.
</div>

This study provides a framework for identifying causal factors of anxiety and depression in college students, with the key results replicating in two distinct cohorts sampled weekly over the course of an academic year. Stress is a causal predictor of anxiety, while low self-esteem is a causal predictor of depression and, to a lesser extent, anxiety. These results support the vulnerability model of depression and suggest that ameliorating high rates of stress may reduce subsequent increases in self-reported anxiety.

[COVID-19, Mental Health and Behavior](http://www.jmir.org/2020/6/e20185/)

The COVID-19 pandemic has impacted the mental health of millions, if not billions of individuals around the world. During the initial stages of the COVID-19 pandemic we characterized mental health and behavioral changes using the StudentLife app. Unsurprisingly, the students we followed were more sedentary, depressed and anxious during this time period.

<img class="col three left" src="https://www.jmir.org/api/download?filename=da72fd19d4fb58b76e89c780afdef2b8.png&alt_name=20185-380580-1-PB.png" alt="" title="Figure 1"/>

<div class="col three caption">
    Sedentary time (top), depression (middle), and anxiety (bottom) scores across an academic term and the first 2 weeks of break, with the term influenced by the outbreak of the COVID-19 pandemic as a separate line. Control terms include data from the same group of individuals across previous academic terms.
</div>

We then leveraged multiple mobile sensing and mental health features to infer the proportion of news stories related to coronavirus over time. A wide variety of behaviors, including increased phone usage, decreased physical activity, and fewer locations visited, among others, were associated with coronavirus news stories.


This project brings together collaborators with expertise in psychiatry, computer science, neuroimaging and social psychology.
