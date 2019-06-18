---
layout: page
title: automated image analysis
description: cell phase duration
img: /assets/img/dcelliq.jpg
---

DCellIQ is a user-friendly software package that is designed for quantitative time-lapse nuclei image analysis for cell cycle studies, whose key features include automated nuclei detection, segmentation, quantification, tracking, cell cycle phase identification, and statistical analysis of the cell cycle duration.


<div class="img_row">
    <img class="col one left" src="{{ site.baseurl }}/assets/img/Normal_Cell_Life_Cycle.png" alt="" title="Cell Cycle 1"/>
    <img class="col one left" src="{{ site.baseurl }}/assets/img/Cell_Cycle_2-2.png" alt="" title="Cell Cycle 2"/>
    <img class="col one left" src="{{ site.baseurl }}/assets/img/dcelliq.jpg" alt="" title="example image"/>
</div>
<div class="col three caption">
     Left: An artists depiction of the cell cycle. Middle: An alternate representation of the cell cycle. Right: DCellIQ segmentation of cell nuclei tagged with H2B-GFP showing various cell cycle phases.
</div>

Initially, a variety of standard machine learning techniques were implemented, including Support Vector Machines (SVM) and Conditional Random Fields, which were further extended with "Online" SVMs which allowed an experimenter to update the model while manually correcting classifier errors. Full text is available <a href="https://academic.oup.com/bioinformatics/article/24/1/94/205039">here</a>.

These methods achieved relatively high accuracy, but the goal of the project was to be able to pick up on small perturbations to the cell cycle due from drugs of other manipulations. As cultured cancel cells such as these (HeLa, MC10) spend most of them time in interphase, any errors in the identification of prophase, metaphase or anaphase have big impacts on estimated durations of cell division.

To potentially improve upon the classification accuracy observed with SVMs and using one image of cells, we took a time-series approach. In hindsight, this is where a Bayesian approach would have been very useful. Instead we generated sets of heuristic rules for a few features which change significantly throughout the cell phase, specifically nucleus area and intensity. Full-text of this approach is available <a href="https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0025511">here</a>.



<img class="col three left" src="https://journals.plos.org/plosone/article/figure/image?size=large&id=10.1371/journal.pone.0025511.g001" alt="" title="Figure 1"/>

<div class="col three caption">
    ‘Area’ and ‘Average Intensity’ features are sufficient to identify the boundaries of mitosis. (a) A portion of an image of HeLa cells expressing the fluorescent marker H2B-GFP is shown. The red asterisk marks an example of a nucleus automatically tracked throughout a division. Images were acquired every 12 minutes. At the time of division (between frames 4 and 5) each daughter nucleus is tracked independently to produce a “trace” for the division. The images of the trace are then used for the time-series analysis as shown in (b). (b) An example of a trace, showing the values of average intensity (I) and area (A) graphed over time with montage of nucleus images. The interphase-prophase transition (IPT) and metaphase-anaphase transition (MAT) points are identified.
</div>

By implementing the time-series approach we were able to increase accuracy to an acceptable level for use in drug screening, with no significant differences identified between performance of the algorithm and a human's rating of the ground truth. This was done using only two human-interpretable features which can facilitate automated analysis of high-throughput time-lapse data sets to identify small molecules or gene products that influence timing of cell division.

Cell cycle images from wikimedia under CC BY-SA 4.0.
