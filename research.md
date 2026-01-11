---
layout: single
title: Research Projects
permalink: /research/
---
## 🌸 Flower Color Index (FCI) {#fci}
Flowers provide substantial ecological and economic benefits, yet their detection and monitoring using remote sensing remain challenging and underexplored. In this study, we introduce the <strong>Flower Color Index (FCI) </strong>, which leverages remote sensing bands sensitive to major flower color pigments—<strong>carotenoids, anthocyanins, and betalains</strong>—to detect four dominant warm flower colors: <strong>red, pink, purple, and yellow</strong>. These pigments primarily influence reflectance in the visible spectrum, enabling FCI to be derived from <strong>widely available blue (B), green (G), red (R), and near-infrared (NIR) bands</strong> across platforms ranging from UAVs to satellites. We demonstrate the application of FCI across species representing diverse vegetation forms (herbaceous plants, shrubs, and trees) and across multiple study locations—including global biodiversity hotspots—using imagery at multiple spatial resolutions (<strong>SkySat, 0.5 m; PlanetScope, 3 m; and Landsat, 30 m</strong>). Results show that FCI effectively detects and quantifies flowering events, supporting applications in ecology (e.g., flowering phenology, species identification, and biodiversity conservation), agriculture (e.g., pollination management and yield estimation), and ecotourism (e.g., cherry blossom festivals). Its simple formulation enables rapid computation and consistent performance across environments, spatial scales, and background conditions.

<figure style="text-align: center; display: inline-block; max-width:800px; width:100%;">
  <a href="{{ site.baseurl }}/assets/images/FCI_StudyArea.png">
    <img src="{{ site.baseurl }}/assets/images/FCI_StudyArea.png"
         alt="Global study areas and flower spectra used to evaluate the Flower Color Index"
         style="width:100%; height:auto;">
  </a>
  <figcaption style="font-size: 0.9em; font-style: italic; text-align: center;">
    Geographic distribution of study areas spanning the Northern and Southern Hemispheres, including the United States, the Atlantic Forest of Brazil and Paraguay, the Netherlands, Nepal, and urban forests in Africa and Australia. The study includes multiple species (California wildflowers, Pleroma, pink trumpet tree, tulip, rhododendron, and jacaranda) and their corresponding flower reflectance spectra.
  </figcaption>
</figure>


<figure>
  {% include slider.html
    id="fci"
    before="Jacaranda_RGB.jpg"
    after="Jacaranda_FCI.jpg"
    before_label="RGB Image"
    after_label="Flower Color Index (FCI)"
  %}
  <figcaption style="font-size: 0.9em; font-style: italic; text-align: center;">
    Comparison between the original RGB image and the Flower Color Index (FCI) result for a jacaranda tree, illustrating the enhancement of flowering signals relative to the background vegetation.
  </figcaption>
</figure>



---

## 🌲 Species Mapping with PlanetScope {#planet}
This project focuses on high-resolution species mapping using PlanetScope imagery.

{% include slider.html
  id="planet"
  before="planet_before.jpg"
  after="planet_after.jpg"
  before_label="Raw imagery"
  after_label="Species classification"
%}

---

## 🌎 Regional-Scale Species Mapping with Landsat {#landsat}
We mapped species at regional-scale using multi-temporal Landsat imagery.

{% include slider.html
  id="landsat"
  before="landsat_before.jpg"
  after="landsat_after.jpg"
  before_label="Baseline"
  after_label="Final species map"
%}

---
[← Back to Home](/)

