---
layout: single
title: Research Projects
permalink: /research/
---
## 🌸 Flower Color Index (FCI) {#fci}
Flowers provide substantial ecological and economic benefits, yet their detection and monitoring using remote sensing remain challenging and underexplored. In this study, we introduce the <strong>Flower Color Index (FCI) </strong>, which leverages remote sensing bands sensitive to major flower color pigments—<strong>carotenoids, anthocyanins, and betalains</strong>—to detect four dominant warm flower colors: <strong>red, pink, purple, and yellow</strong>. These pigments primarily influence reflectance in the visible spectrum, enabling FCI to be derived from <strong>widely available blue (B), green (G), red (R), and near-infrared (NIR) bands</strong> across platforms ranging from UAVs to satellites. We demonstrate the application of FCI across species representing diverse vegetation forms (herbaceous plants, shrubs, and trees) and across multiple study locations—including global biodiversity hotspots—using imagery at multiple spatial resolutions (<strong>SkySat, 0.5 m; PlanetScope, 3 m; and Landsat, 30 m</strong>). Results show that FCI effectively detects and quantifies flowering events, supporting applications in ecology (e.g., flowering phenology, species identification, and biodiversity conservation), agriculture (e.g., pollination management and yield estimation), and ecotourism (e.g., cherry blossom festivals). Its simple formulation enables rapid computation and consistent performance across environments, spatial scales, and background conditions.

<!-- Container for the two panels -->
<div style="display: flex; justify-content: space-between; width: 80%; margin: 0 auto; gap: 20px; align-items: stretch;">

  <!-- Panel 1: Study Area (60%) -->
  <figure style="flex: 0 0 45%; display: flex; flex-direction: column;justify-content:centers; /*vertically center figure+caption */; align-items: center; text-align: center; margin: 0; border: 1px solid #ccc; border-radius: 5px; padding: 5px; box-sizing: border-box;">

    <!-- Image wrapper to center the image -->
    <div style="flex: 1; display: flex; justify-content: center; align-items: center; width: 100%;">
      <a href="{{ site.baseurl }}/assets/images/FCI_StudyArea.png" style="display: flex; justify-content: center; align-items: center; width: 100%; height: 100%;">
        <img src="{{ site.baseurl }}/assets/images/FCI_StudyArea.png"
             alt="Global study areas and flower spectra used to evaluate the Flower Color Index"
             style="max-width: 100%; max-height: 100%; object-fit: contain; display: block;">
      </a>
    </div>

    <!-- Caption -->
    <figcaption style="font-size: 0.9em; font-style: italic; line-height: 1.3; margin-top: 4px; margin-bottom: 0; padding: 0;">
       Geographic locations of study areas across the globe spanning northern and southern hemispheres (United States, a biodiversity hotspot from North America;the Atlantic Forest of Brazil, a biodiversity hotspot, and Paraguay from South America; Holland, thelargest tulip bulb producer in the world from Europe; Nepal, a biodiversity hotspot from Asia; urban forests from Africa and Australia) and species (California’s wildflowers, Pleroma, pink trumpet, tulip, rhododendron, and jacaranda) used in the study (a) and spectra of respective flowers (b). Flowering sample polygons were used to extract flower spectral reflectance across bands corresponding to satellite imagery acquired during the bloom; the number and types of bands (coastal blue [C], blue [B], green [G], red [R], near-infrared [NIR], shortwave infrared 1 [S1], and shortwave infrared 2 [S2]) varied among satellite sensors (SkySat [0.5 m; 4 bands], PlanetScope [3 m; 4 bands], and Landsat [30 m; 7 bands]). Each line shows the mean surface reflectance (Y-axis) ± one standard deviation across spectral bands (X-axis). Dashed, solid, and dotted lines represent SkySat, PlanetScope, and Landsat data, respectively.
    </figcaption>

  </figure>

  <!-- Panel 2: Slider (40%) -->
  <figure style="flex: 0 0 55%; display: flex; flex-direction: column; text-align: center; margin: 0; border: 1px solid #ccc; border-radius: 5px; padding: 5px; box-sizing: border-box;">

    <!-- Slider wrapper -->
    <div style="flex: 1; display: flex; justify-content: center; align-items: center; width: 100%;">
      {% include slider.html
        id="fci"
        before="Jacaranda_RGB.jpg"
        after="Jacaranda_FCI.jpg"
        before_label="RGB Image"
        after_label="Flower Color Index (FCI)"
      %}
    </div>

    <!-- Caption -->
    <figcaption style="font-size: 0.9em; font-style: italic; line-height: 1.3; margin-top: 4px; margin-bottom: 0; padding: 0;">
      Comparison between the original RGB image and the Flower Color Index (FCI) result for a jacaranda tree.
    </figcaption>

  </figure>

</div>


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

