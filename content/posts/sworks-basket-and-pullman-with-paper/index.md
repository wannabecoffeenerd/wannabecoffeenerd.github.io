---
title: "More baskets, bottom paper filters and the \"volcano\" effect"
date: 2023-03-18T16:00:00-08:00
draft: false
_build:
  render: always
  list: false
  publishResources: true

categories: ["theory", "espresso"]
tags: ["evenness", "espresso", "wafo", "sworksdesign", "pullman", "bottom paper filter", "puck prep"]
featuredImage: "images/schematic.svg"
featuredImagePreview: "images/schematic.svg"
description: "A look at the \"volcano\" effect and the effect that edge extraction has on it by comparing extractions using a Pullman basket with those from a WAFO basket."
---

<!--more-->

In my [earlier post](http://www.caffeinated.science/posts/edge-extraction-wafo/), I compared a WAFO SOE Spirit espresso basket to a Pullman basket to see how basket design affects edge extraction. One question that came up a lot was how would a precision basket like the WAFO compare with the Pullman basket with the use of bottom paper filters. Another question that came up was how would another precision basket like the [Sworksdesign billet basket](https://sworksdesign.com/Billet-Basket-Pre-order-p515767358). This is a follow up post trying to answer some aspects of these questions.

## Sworksdesign basket

At the outset, I should mention that the Sworksdesign basket that I used here was a pre-production model that Sheldon from Sworksdesign let me borrow for a few weeks. From what I gather, this pre-production model was somewhere in between the standard and high-flow variants.

{{< image src="images/wafo_sworks_hole_dia.jpg" caption="Bottom hole area of the WAFO SOE Spirit and the Sworksdesign basket compared." >}}

## Extraction measurements

The experiment process here is the same as the [last post](http://www.caffeinated.science/posts/edge-extraction-wafo/). I ground and prepped pucks with different grind settings on my P100 with the Pre-2015 EK43 burr geometry manufactured by SSP. All shots were pulled on a Decent Espresso DE1 with a [flat 6 bar profile](https://visualizer.coffee/shots/aafb4a69-03a0-48d1-bb84-498171866e67). The coffee I used for this experiment was the same [Worka Site](https://www.seycoffee.com/products/worka-site) from SEY coffee that was used in the previous post. For all the results, I plotted burr gap instead of the grind setting using the conversion factor of 75 microns per large tick on the P100.

In addition to the Sworksdesign basket described above, I also tested with a Pullman 17-19g basket with bottom paper filters. The filters were bleached Chemex filters cut using a punch cutter with a 57.15 mm diameter. For brevity, I will refer to this as Pullman+paper. No bottom paper filters were used with the Sworksdesign basket.

### Results

First, we can compare the Sworksdesign basket to the Pullman+paper setup in terms of extraction yield (EY) plotted against burr gap below:

{{< image src="data/sworksdesign_pullman_paper_extraction_yield.png" caption="Extraction yield vs. burr gap (grind setting, lower is finer) with the Sworksdesign and Pullman+paper baskets." >}}

We still see the "volcano" effect here for both baskets. However, the peak is very fine for both setups with pretty high extraction yields, in excess of 28%. The peak EY point with Pullman+paper is slightly coarser compared to the Sworksdesign basket. The peak EY values for both baskets are very similar with the Sworksdesign peak being very slightly higher than the Pullman+paper peak.

The plot below shows the shot time for both baskets:

{{< image src="data/sworksdesign_pullman_paper_shot_time.png" caption="Shot time vs. burr gap (grind setting, lower is finer) with the Sworksdesign and Pullman+paper baskets." >}}

### Comparison to previous results

A natural question is how do the basket setups from the above section compare to the ones from the previous post. It is not easy to draw meaningful conclusions from two separate experiments even if the setup remains constant due to factors that cannot be controlled perfectly. Probably the biggest of these factors are the beans themselves and potential aging between the two experiments even though the same beans from the same batch were used for both experiments and I froze the beans right after the previous experiment and thawed them a few hours before this experiment. To test this, I pulled a shot with the same grind as with the previous WAFO peak and compared it against the earlier results as plotted below:

{{< image src="data/wafo_compare_extraction_yield.png" caption="Extraction yield vs. burr gap (grind setting, lower is finer) with the WAFO SOE Spirit basket. Green markers are the earlier results and blue is the result from this experiment" >}}

The result from this experiment is in very good agreement with the previous results indicating that any factors that might have changed between the two experiments are not very significant. With this result, we can (cautiously) try to compare all four setups.

{{< image src="data/all_baskets_extraction_yield.png" caption="Extraction yield vs. burr gap (grind setting, lower is finer) with all baskets used." >}}

{{< image src="data/all_baskets_shot_time.png" caption="Shot time vs. burr gap (grind setting, lower is finer) with all baskets used." >}}

Comparing all four basket setups together is very interesting. It would seem that it was just coincidence that the EY peak for Pullman and the WAFO baskets were at the same grind size. Or the WAFO was optimized to have similar resistance as a standard basket maybe? With bottom filters, the Pullman basket has much higher EY at a much finer grind size. The Sworksdesign basket has a slightly higher peak EY still and an even finer peak. Even in terms of shot times, the WAFO is a fair bit slower than Pullman+paper or the Sworksdesign basket.

## Conclusion

From the results above, the main conclusion to draw is that bottom paper filters with the Pullman basket can have a huge impact in terms of extraction, up to 3% higher with bottom filters and similar extractions compared to newer precision baskets like the WAFO and Sworksdesign. The WAFO basket fixes edge underextraction pretty well, but has higher basket resistance compared to Pullman+paper and Sworksdesign baskets and therefore has an EY peak at a much coarser grind. The Sworksdesign basket has its EY peak at a very very fine grind and at a fairly long shot time. This has potential implications in terms of flavor modulation and preferential extraction and whether or not this is desirable from a taste standpoint depends a lot on taste preferences and other factors.
