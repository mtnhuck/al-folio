---
layout: page
title: Reward
description: reward and self-regulation
img: /assets/img/reward_cloud.png
---

Reward plays a critical role in motivating approach behaviors while self-regulation inhibits maladaptive or overactive approach behaviors. For my dissertation work I focused on connectivity from reward-related regions, and how these and other regions interact. Strong resting-state functional connectivity of the nucleus accumbens was observed in ventromedial prefrontal regions along with other subcortical areas.
<div class="img_row">
    <img class="col three left" src="{{ site.baseurl }}/assets/img/NAcc_conn.png" alt="" title="NAcc_conn"/>
</div>
<div class="col three caption">
    Nucleus accumbens resting-state functional connectivity map
</div>
<div class="img_row">
    <img class="col three left" src="{{ site.baseurl }}/assets/img/reward_cloud.png" alt="" title="NAcc_conn"/>
</div>
<div class="col three caption">
    Similarity of NAcc maps to terms in Neurosynth
</div>

 The NAcc connectivity map was submitted to Neurosynth for reverse inference of pattern similarity against large-scale meta-analyses of other fMRI studies. Terms of reward-related behavior loaded highly and can be observed in the word-cloud above. Now, just because NAcc connectivity is similar to brain patterns associated with reward processing, it doesn't mean that we can say there is a reward network yet. To test if there is a distinct reward network a graph theoretical community assignment algorithm was used.
 <div class="img_row">
     <img class="col three left" src="{{ site.baseurl }}/assets/img/reward_graph.png" alt="" title="Community Assignments"/>
 </div>
 <div class="col three caption">
     Community assignment reveals a distinct reward network
 </div>
By viewing connections between all brain regions selected at once it is possible to get an idea if some regions are preferentially connected. Community assignment is a way to do this and the Infomap algorithm was implemented. Basically this takes connectivity between all regions, and thresholds it, removing weak connections. Then a random walk moving around the graph (network) is performed many times, seeing how often different regions cluster together. This is repeated at many thresholds. By adding nucleus accumbens and to a set of regions lovingly referred to as to as "big brain" (Powers, et al., 2001) and modifying some of those regions to be closer to reward-related peaks we observed a set of regions which were preferentially coupled, which appear to be a reward-related network.

https://www.jonathanpower.net/2011-neuron-bigbrain.html

The applications for a predefined reward network are wide. Work by Lopez et al (2017) looked at the balance of control network and reward network activation during a food cue-reactivity task. This ratio of control to reward activity predicted subsequent eating behaviors reported through ecological momentary assessments. These results held up with both anatomical reward regions (NAcc) and the above-defined reward network.

More information coming soon!
