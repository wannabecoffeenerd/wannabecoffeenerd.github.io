---
title: "Edge extraction, \"volcano\" effect and better baskets"
date: 2022-12-31T20:16:42-08:00
draft: true
_build:
  render: always
  list: true
  publishResources: true

categories: ["theory", "espresso"]
tags: ["evenness", "espresso", "wafo", "puck prep"]
featuredImage: "images/schematic.svg"
featuredImagePreview: "images/schematic.svg"
description: "A look at the \"volcano\" effect and the effect that edge extraction has on it by comparing extractions using a Pullman basket with those from a WAFO basket."
---

<!--more-->

The [turbo paper](https://www.cell.com/matter/fulltext/S2590-2385(19)30410-2) introduced the concept of the "volcano" effect. This is essentially a statement about the trade-off between finer grinds causing an increase in extraction yield but only to a certain extent. Going too fine causes _channeling_ that then reduces bulk extraction yield due to uneven extraction. The paper has some really nice ideas about modeling extraction, and the discrepancy between the model prediction and the experimental results were attributed to _channeling_. The experiments in the paper used a VST basket without any bottom paper filters. For a while now, I have been wondering if that volcano effect is really a manifestation of _channeling_ as is usually thought of (general [lateral unevenness](https://www.caffeinated.science/posts/espresso-extraction-evenness/#lateral-unevenness)) or if it is really a manifestation of [edge underextraction](https://www.caffeinated.science/posts/espresso-extraction-evenness/#edge-underextraction) stemming from the blank areas without holes on espresso basket edges.

{{< image src="images/schematic.svg" caption="Schematic theorizing why blank basket edges cause edge underextraction." >}}

I got the chance to try out the WAFO espresso baskets recently (courtesy of [Brian Quan](https://www.youtube.com/@BrianQuan)) and thought this would be a great way to test out this hypothesis. Specifically, I used the WAFO SOE Spirit basket that has holes that go very close to the basket edge as well as being slit shaped instead of the standard circular holes.

## WAFO basket

WAFO make 4 baskets. Two of them are labeled SOE for Single Origin Espresso and the other two are labeled Blend. For this post, I was mainly interested in looking at the SOE baskets since they have the edge to edge holes promising to mitigate edge underextraction. After some initial testing, the SOE Spirit basket looked to have the most even puck bottoms and the SOE Classic basket had a very tiny bit of edge discoloration of spent puck bottoms. For the rest of this post, I will only discuss the SOE Spirit basket.

{{< image src="images/wafo_soe_spirit.jpg" caption="WAFO SOE Spirit basket with slit shaped holes going very close to the edge." >}}

## Extraction measurements

The experiment here is simple. I ground and prepped pucks with different grind settings on my P100 with the Pre-2015 EK43 burr geometry manufactured by SSP. All shots were pulled on a Decent Espresso DE1 with a flat 6 bar profile. The coffee I used for this experiment was the [Worka Site](https://www.seycoffee.com/products/worka-site) from SEY coffee. For all the results, I plotted the burr gap instead of the grind setting using the conversion factor of 75 microns per large tick on the P100. Shots were pulled using the WAFO SOE Spirit basket and with a Pullman 17-19g basket for comparison.

### Puck prep

The puck prep process I used was as follows:

1. Grind a set dose of coffee.
2. Dose into a basket, weigh the ground coffee, no bottom paper filters.
3. Deep WDT with the 4z level method as described in [this video](https://youtu.be/HMo-2sZ42bY) followed very light vertical tap.
5. Tamp with a Normcore V3 tamper that I modded with a 25 lb internal spring for a level and calibrated tamp.
6. Add a top Aeropress filter for cleanliness (this was not my machine). I didn't use a Flair 58 screen since there have been some reports of the Flair screen affecting edge extraction and didn't want to add that additional variable to this experiment.

### Results

Here is the main result. The plot below shows the extraction yield as a function of gring burr gap:

{{< image src="data/wafo_pullman_extraction_yield.png" caption="Extraction yield vs. burr gap (grind setting, lower is finer) with the WAFO and Pullman baskets." >}}

We clearly see the "volcano" effect here for both baskets. Starting on the right with the coarsest grind, extraction is limited by just the exposed surface area and so the effect of the basket is not significant. As we go finer (left in the plot), more surface area is exposed causing extraction to increase. After a certain point, extraction starts dropping again because of unevenness.



Comparing the two baskets, the WAFO enables much higher extractions. The WAFO peak is almost 2.5% higher EY than the Pullman indicating that the Pullman is limited by edge underextraction. This is reflected in puck bottom images as well.

{{< image src="images/wafo_puck_bottoms.jpg" caption="Images of post extraction puck bottoms with the WAFO basket. Finest grind setting on the left, peak extraction on the right." >}}

{{< image src="images/pullman_puck_bottoms.jpg" caption="Images of post extraction puck bottoms with the Pullman basket. Finest grind setting on the left, peak extraction on the right." >}}

At the volcano peak (right half in the images above), the WAFO puck bottom is perfectly even but the Pullman puck has dark edges indicating edge underextraction. This edge underextraction is why the Pullman has a lower bulk extraction yield compared to the WAFO basket. At the finest grind setting (left half in the images above), both baskets show signs of unevenness in the center of the puck but the Pullman has edge underextraction here as well.

Interestingly, both baskets have the extraction peak at the same grind setting. This indicates that though the Pullman has edge underextraction, it isn't sufficient to reduce bulk extraction.

## Conclusion

The aim of this experiment was to look at the role of edge underextraction in the "volcano" effect. The results suggest that edge underextraction is indeed the first EY limiter when going from coarse to fine, but it isn't sufficient to cause the volcano effect itself. The reduction in EY at very fine grind stems from more broad unevenness or _channeling_. The other more practical conclusion is that the WAFO SOE Spirit basket does indeed do a very good job at mitigating edge underextraction. Practically, this means that one can forgo bottom paper filters without worrying about that slight harshness that comes from uneven extraction.
