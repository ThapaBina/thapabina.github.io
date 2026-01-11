---
layout: single
title: Research Projects
permalink: /research/
---
<h3>🌸 Flower Color Index (FCI)</h3>
<div class="project-text-box" style="background-color: red; border: 5px solid yellow;">
  <p>
    Flowers provide substantial ecological and economic benefits, yet their detection and monitoring using remote sensing remain challenging and underexplored. In this study, we introduce the <strong>Flower Color Index (FCI)</strong>, which leverages remote sensing bands sensitive to major flower color pigments—<strong>carotenoids, anthocyanins, and betalains</strong>—to detect four dominant warm flower colors: <strong>red, pink, purple, and yellow</strong>. These pigments primarily influence reflectance in the visible spectrum, enabling FCI to be derived from <strong>widely available blue (B), green (G), red (R), and near-infrared (NIR) bands</strong> across platforms ranging from UAVs to satellites. We demonstrate the application of FCI across species representing diverse vegetation forms (herbaceous plants, shrubs, and trees) and across multiple study locations—including global biodiversity hotspots—using imagery at multiple spatial resolutions (<strong>SkySat, 0.5 m; PlanetScope, 3 m; and Landsat, 30 m</strong>). Results show that FCI effectively detects and quantifies flowering events, supporting applications in ecology, agriculture, and ecotourism. Its simple formulation enables rapid computation and consistent performance across environments, spatial scales, and background conditions.
  </p>
</div>


<!-- Container for the two panels -->
<div style="display: flex; justify-content: space-between; width: 80%; margin: 0 auto; gap: 20px; align-items: stretch; padding: 0;">

  <!-- Panel 1: Study Area (45%) -->
  <figure style="
    flex: 0 0 45%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    margin: 0;
    border: 1px solid #ccc;
    border-radius: 5px;
    padding: 0; /* Removed padding to reduce top/bottom space */
    box-sizing: border-box;
    position: relative;
  ">

    <!-- Image wrapper -->
    <div style="
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      position: relative;
      margin: 0;
      padding: 0;
    ">
      <!-- Image link -->
      <a href="{{ site.baseurl }}/assets/images/FCI_StudyArea.png" target="_blank"
         style="display: block; position: relative; width: 100%; margin: 0; padding: 0;">
        
        <!-- Image -->
        <img src="{{ site.baseurl }}/assets/images/FCI_StudyArea.png"
             alt="Global study areas and flower spectra used to evaluate the Flower Color Index"
             style="display: block; width: 100%; height: auto; object-fit: contain; margin: 0; padding: 0;">

        <!-- Zoom icon overlay -->
        <span class="zoom-icon" 
              style="position: absolute; top: 8px; right: 8px; background: rgba(0,0,0,0.6); color: white; padding: 4px 6px; border-radius: 3px; font-size: 1.2em; cursor: pointer; opacity: 0; transition: opacity 0.2s; z-index: 10;">
          🔍
        </span>

      </a>
    </div>

    <!-- Caption directly below image -->
    <figcaption style="
      font-size: 0.9em;
      font-style: italic;
      line-height: 1.3;
      justify-content: center;
      margin: 2px 0 0 0; /* very small top margin to reduce gap */
      padding: 0;
    ">
      Geographic locations of study areas across the globe spanning northern and southern hemispheres (United States, a biodiversity hotspot from North America; the Atlantic Forest of Brazil, a biodiversity hotspot, and Paraguay from South America; Holland, the largest tulip bulb producer in the world from Europe; Nepal, a biodiversity hotspot from Asia; urban forests from Africa and Australia) and species (California’s wildflowers, Pleroma, pink trumpet, tulip, rhododendron, and jacaranda) used in the study and spectra of respective flowers. Flowering sample polygons were used to extract flower spectral reflectance across bands corresponding to satellite imagery acquired during the bloom; the number and types of bands (coastal blue [C], blue [B], green [G], red [R], near-infrared [NIR], shortwave infrared 1 [S1], and shortwave infrared 2 [S2]) varied among satellite sensors (SkySat [0.5 m; 4 bands], PlanetScope [3 m; 4 bands], and Landsat [30 m; 7 bands]). Each line shows the mean surface reflectance ± one standard deviation across spectral bands. Dashed, solid, and dotted lines represent SkySat, PlanetScope, and Landsat data.
    </figcaption>

  </figure>

  <!-- Panel 2: Slider (55%) -->
  <figure style="
    flex: 0 0 55%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    margin: 0;
    border: 1px solid #ccc;
    border-radius: 5px;
    padding: 0; /* Removed padding to reduce white space */
    box-sizing: border-box;
  ">

    <!-- Slider wrapper -->
    <div style="
      flex: 1;
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100%;
      margin: 0;
      padding: 0;
      position: relative;
    ">
      {% include slider.html
        id="fci"
        before="Jacaranda_RGB.jpg"
        after="Jacaranda_FCI.jpg"
        before_label="RGB Image"
        after_label="Flower Color Index (FCI)"
      %}
    </div>

    <!-- Caption -->
    <figcaption style="
      font-size: 0.9em;
      font-style: italic;
      line-height: 1.3;
      margin: 2px 0 0 0; /* reduce space between slider and caption */
      padding: 0;
    ">
      Visualization of Jacaranda bloom using the Flower Color Index (FCI)-Purple applied to RGB imagery.
    </figcaption>

  </figure>

</div>

<!-- CSS for hover zoom icon -->
<style>
  figure a:hover .zoom-icon {
    opacity: 1;
  }

  /* make cursor pointer for image */
  figure a {
    cursor: zoom-in;
  }
</style>


<!-- Publications Section -->
<h4 class="pub-heading">Publication</h4>
<div class="publication-list">
  Thapa, B., Hardiman, B. S., & Fei, S. (2025).
  Flower color index for detecting and monitoring warm-colored flowering across scales.<em>
  International Journal of Applied Earth Observation and Geoinformation </em>, 145, 104978.
  <a href="#">Link</a>
</div>

---

## 🌲 Species Mapping with PlanetScope {#planet}
This project focuses on high-resolution species mapping using PlanetScope imagery.
<div style="text-align: left; margin: 20px 0;">
  <strong style="font-style: italic; color: #555;">Details are coming soon!</strong>
</div>

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

<div style="text-align: left; margin: 20px 0;">
  <strong style="font-style: italic; color: #555;">Details are coming soon!</strong>
</div>


{% include slider.html
  id="landsat"
  before="landsat_before.jpg"
  after="landsat_after.jpg"
  before_label="Baseline"
  after_label="Final species map"
%}

---
[← Back to Home](/)

