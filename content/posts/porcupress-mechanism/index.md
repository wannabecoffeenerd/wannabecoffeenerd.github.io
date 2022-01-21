---
title: "What does the Hog/Porcupress really do?"
date: 2022-01-18T20:16:42-08:00
draft: false
_build:
  render: always
  list: true
  publishResources: true

categories: ["theory", "espresso"]
tags: ["evenness", "espresso", "porcupress", "hog", "puck prep"]
featuredImage: "images/schematic.svg"
featuredImagePreview: "images/schematic.svg"
description: "Experiments with the hog/porcupress measuring tamped puck density and extraction yields to try and deduce how it really works and affects extraction."
---

<!--more-->

There has been a lot of discussion about the [PorcuPress](https://sworksdesign.com/PorcuPress-p379522166) recently in many coffee forums. Many people have reported improved extractions and taste benefits of using the PorcuPress in their puck prep routine. However, the PorcuPress is not the first of its kind. This type of device has been around for a while and was explored by Michael Cameron and Matt Perger back in 2017. They called it "The Hog" and introduced it in [this video](https://youtu.be/tS0c3ZCtVZs). The video is a great watch since they not only discuss the Hog, but also some ideas that will eventually develop into the [turbo paper](https://www.cell.com/matter/fulltext/S2590-2385(19)30410-2).

The Hog/PorcuPress is fundamentally an array of needles that is used to stab a prepped but untamped dose of coffee in a portafilter. This is typically done after WDT. What it does not involve is any spinning or movement of the tool. It just creates holes and then the puck is tamped as is. So how does it work and what does it do?

The conventional wisdom as to why the Hog/PorcuPress works is described well by this excerpt from the PorcuPress product page:

> The PorcuPress is here to help reduce channeling, specifically on very  finely ground coffee. The tool perforates the coffee puck such that  after you tamp, you will leave behind a defined array of less compacted  regions. These regions will initially allow water through the entire  depth of the puck. Water will then saturate outwards from each of these  holes causing the entire puck of coffee to be fully wet. As the entire  puck swells, these holes and other naturally present channels will seal  up.

So the idea is that the holes that the tool creates remain low density regions after tamping. And this serves to better wet your puck during pre-infusion or provide more even percolation pathways leading to an overall more even extraction.

But is this really what this tool does? That's the question I tried to answer with the two sets of experiments below.

## Puck density measurements

Recently, I came across this really simple and elegant way of measuring tamped puck thickness and density by Michael Cooper in their [Quantitative Cafe](https://quantitativecafe.com/2021/10/17/measuring-density/) blog. Michael also designed a neat [3D printed accessory](https://www.thingiverse.com/thing:5023407) to attach to a set of digital calipers. My first thought was to try and use this method of measuring puck density to try and deduce what the Hog/PorcuPress is really doing. Going by the conventional theory of how the Hog/PorcuPress works, low density regions created in a tamped puck should reduce the overall puck density compared to a puck prepped and tamped without use of the Hog/PorcuPress.

The experiment here is fairly simple. I ground some coffee and prepped pucks with and without the PorcuPress and measured puck thickness and density for them. The coffee I used for this experiment was the [Pepe Arguello](https://www.seycoffee.com/products/pepe-arguello) from SEY coffee. The grinder I used was a DF64 with the SSP Multipurpose burrs set at grind setting 4.

### Puck prep

The puck prep process I used was as follows:

1. Grind a set dose of coffee
2. Dose into a Pullman 17-19g basket, weigh the ground coffee
3. Deep WDT with the 4z level method as described in [this video](https://youtu.be/HMo-2sZ42bY) followed very light vertical tap
4. PorcuPress if required for that trial. The PorcuPress I used had the standard density offset square configuration and I did two rounds with a 180° rotational offset to effectively double the number of holes made in the pre-tamped puck.
5. Tamp with a Normcore V3 tamper that I modded with a 25 lb internal spring for a level and calibrated tamp.
6. Place the [Flair 58 screen](https://flairespresso.com/product/flair-58-puck-screen/) and tamp again. The reason I used the Flair 58 screen was to prevent the depth measurement insert on the calipers from digging into the puck and therefore underestimating the puck thickness. Also, see [this article](https://quantitativecafe.com/2021/12/29/a-closer-look-at-tamping/) for a more in depth look at what tamping multiple times does.

{{< image src="images/puck_prep.jpg" caption="Image of the post WDT bed on the left and post PorcuPress bed on the right. Notice all the holes created by the PorcuPress needles on the right." >}}

### Density measurement methodology

After prepping the puck, I made puck thickness and density measurements as follows:

1. Measure the depth of the top of the Flair 58 screen from the top of the basket
2. Knock the puck out, wipe the basket clean and measure the depth of the basket bottom from the top of the basket. This value should be the same for a given basket, but measuring this for every trial accounts for any zeroing errors that might crop up from the depth measurement accessory slipping on the caliper frame between trials. Care was taken to handle the calipers very gently during a trial.
3. Get puck thickness by subtracting the depth of the top of the Flair screen and the thickness of the Flair screen from the depth of the basket bottom.
4. Get puck density by assuming a cylindrical shape with radius matching the basket diameter. This is not completely accurate since most baskets have a taper close to the bottom. The Pullman 17-19g basket has very straight walls and only a small taper so this error is limited. But we're only comparing puck density measurements with the same process and basket rather than using absolute density measurements in this article, so this systematic error will just be a constant offset and not change any conclusions that we draw from comparing density measurements.

### Results

Here are the results. The plot below shows the puck thickness for 4 pucks each with and without the porcupress:

{{< image src="data/porcupress_puck_thickness.png" caption="Puck thickness with and without the PorcuPress for 4 different trials." >}}

And the corresponding puck density plot is shown below:

{{< image src="data/porcupress_puck_density.png" caption="Puck density with and without the PorcuPress for 4 different trials." >}}

These results are very interesting since they show that tamped puck density **increases** with the PorcuPress. This increase in density is also significant in that it is higher than puck to puck variance and any variance arising from measurement methodology.

This seems to contradict the idea that a PorcuPress'd puck retains low density areas post tamp. Instead, what it seems to be doing is to allow the puck to settle into a higher density configuration with lower spatial density variations. There are two hypotheses for how this happens:

1. The PorcuPress needles break up higher density regions in the pre-tamped puck with disproportionately larger expected change. As a result, this would reduce the total density variance. This hypothesis seems unlikely though.
2. Holes in the pre-tamped puck created by the PorcuPress  add a degree of freedom for particle movement during tamping that allows them to settle into a higher density configuration than directly tamping. This seems like the more likely hypothesis.

A third hypothesis might be that pushing the needles into the pre-tamped bed would have a lateral/horizontal compression effect and this causes the density increase. Let's try and estimate the volume displaced by these needles compared to the volume of the puck. This ratio is the ratio if the combined cross sectional area of the needles to the cross sectional area of the puck.
$$ \frac{V_\mathrm{needles}}{V_\mathrm{basket}} = \frac{D_\mathrm{needles}^2 N_\mathrm{needles}}{D_\mathrm{basket}^2} = \frac{0.8^2 \times 100 }{58.5^2} \approx 0.019 $$
So, the total volume displaced is only 1.9% of the untamped coffee grounds volume. This estimate would suggest that the lateral compression mechanism is unlikely. While using the PorcuPress, I also noticed that the holes created in the first pass remained intact after the second pass with a 180° rotational offset. This also indicates there isn't significant lateral compression.


## Pulling shots and evaluating extraction 

So far, we've inferred that the PorcuPress does not really create low density _controlled channels_ as a mechanism to improve extraction evenness. Instead, it increases puck density and reduce spatial density variance in tamped pucks. This should allow for more even extraction, especially on the finer end of the spectrum. To test this, I pulled some shots with the [H+S Ecuador Galo Morales Flores](https://hscoffeeroasters.com/products/ecuador-galo-morales-flores) coffee.

### Shot parameters

I pulled shots on my Breville Dual Boiler that has the [flow control mod](https://qporzk.github.io/BDB-Slayer/Modifications/SlayerMod/). I pulled shots at the finer end of the spectrum resulting in ~40s shot times. These slower shots are inherently more prone to uneven extraction and should highlight the effect of the PorcuPress. All shots were pulled with a bottom paper filter (Chemex filters cut to 2.25" diameter circles) to improve evenness and the rest of the puck prep routine was the same as in the previous section. I used a dynamic bloom characteristic profile for all shots which involves a fast 7ml/s fill up to 7 bar, 0 flow until the pressure drops to 2 bar and then ramp flow up to  reach a peak pressure of 7 bar declining to 3-4 bar.

### Results

All shots in this section were pulled at a grind setting of 5 on my DF64. The plot below shows the extraction yield (EY) with and without the PorcuPress:

{{< image src="data/porcupress_extraction_yield.png" caption="Extraction Yield (EY) with and without the PorcuPress for 3 different trials." >}}

PorcuPress shots have higher EY on average and much lower variance. This is directly related to evenness of extraction as evidenced by the images of the post extraction puck bottoms below:

{{< image src="images/puck_bottoms.png" caption="Images of the bottom of the post extraction puck bottoms. Without PorcuPress on the left, with PorcuPress on the right." >}}

One interesting detail from the data is that the PorcuPress shots ran a little faster on average compared to without.

{{< image src="data/porcupress_shot_time.png" caption="Shot times with and without the PorcuPress for 3 different trials." >}}

This might be why the low density controlled channeling idea is popular. The puck density results indicate otherwise though. An explanation for why this is happening might be that PorcuPress allows the puck to settle into a higher density configuration with less density variance and as a result allow for more even extractions. This also means that the extractions are faster and front loaded causing a faster decline in the viscosity of the medium and as a result faster flow towards the end.

Here is the data for all the shots pulled:

| Dose (g) | Time (s) | Notes           | Yield (g) | TDS (%) | EY (%) | Ratio |
| -------- | -------- | --------------- | --------- | ------- | ------ | ----- |
| 16.1     | 44       | No PorcuPress   | 40.5      | 9.01    | 22.66  | 2.52  |
| 16.1     | 41       | With PorcuPress | 41.2      | 9.53    | 24.39  | 2.56  |
| 16.1     | 43       | No PorcuPress   | 40.5      | 9.11    | 22.92  | 2.52  |
| 16.1     | 40       | With PorcuPress | 40.9      | 9.58    | 24.34  | 2.54  |
| 16.1     | 38       | No PorcuPress   | 40.9      | 9.73    | 24.72  | 2.54  |
| 16.1     | 33       | With PorcuPress | 40.9      | 9.80    | 24.90  | 2.54  |

### Coarser/Faster shots

If we go coarser to a grind setting of 6.5, the shots are much faster and as a result much more even in their extractions. In this regime, the difference between using the PorcuPress or not is almost non-existent:

| Dose (g) | Time (s) | Notes           | Yield (g) | TDS (%) | EY (%) | Ratio |
| -------- | -------- | --------------- | --------- | ------- | ------ | ----- |
| 16.2     | 26       | No PorcuPress   | 41.5      | 9.37    | 24.00  | 2.56  |
| 16.2     | 23       | With PorcuPress | 41.5      | 9.36    | 23.98  | 2.56  |

{{< image src="images/puck_bottoms_coarse.png" caption="Images of the bottom of the post extraction puck bottoms with a coarser grind setting. Without PorcuPress on the left, with PorcuPress on the right." >}}

When shots without the PorcuPress already have even extraction, the PorcuPress does not provide any additional benefit from a macroscopic extraction standpoint.

## Conclusion

The main aim of these experiments was to test out the low density controlled channeling theory for why the PorcuPress works. Puck density measurements showed that there is a significant _increase_ in tamped puck density with the PorcuPress. This seems to indicate that the PorcuPress allows for the tamped pucks to settle into a higher density configuration with less density variance rather than creating an even array of low density areas.

Measurements of extraction yield showed that the PorcuPress helps make extractions more even with a higher extraction yield on average and much reduced variance. This means shots with the PorcuPress are likely to be more consistent. This benefit was absent when pulling faster shots, but the PorcuPress does not  seem to hurt extractions in any way. Overall, using the PorcuPress is always a net win.
