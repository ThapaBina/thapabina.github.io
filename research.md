---
layout: single
title: Research Projects
permalink: /research/
---

<h3>🌸 Flower Color Index (FCI)</h3>
<div class="project-text-box" style="width:98%; margin:0 auto;">
  <p>
    Flowers provide substantial ecological and economic benefits, yet their detection and monitoring using remote sensing remain challenging and underexplored. In this study, we introduce the <strong>Flower Color Index (FCI)</strong>, which leverages remote sensing bands sensitive to major flower color pigments—<strong>carotenoids, anthocyanins, and betalains</strong>—to detect four dominant warm flower colors: <strong>red, pink, purple, and yellow</strong>. These pigments primarily influence reflectance in the visible spectrum, enabling FCI to be derived from <strong>widely available blue (B), green (G), red (R), and near-infrared (NIR) bands</strong> across platforms ranging from UAVs to satellites. We demonstrate the application of FCI across species representing diverse vegetation forms (herbaceous plants, shrubs, and trees) and across multiple study locations—including global biodiversity hotspots—using imagery at multiple spatial resolutions (<strong>SkySat, 0.5 m; PlanetScope, 3 m; and Landsat, 30 m</strong>). Results show that FCI effectively detects and quantifies flowering events, supporting applications in ecology, agriculture, and ecotourism. Its simple formulation enables rapid computation and consistent performance across environments, spatial scales, and background conditions.
  </p>
</div>

<div style="width 80%; text-align: left; margin: 20px auto;">
  <strong>
    <em style="color: #555; font-size: 0.8em;">
      The figures below show the global distribution of the study area and an example of FCI-purple detecting Jacaranda bloom in Africa.
    </em>
  </strong>
</div>

<!-- Container for the two panels -->
<div style="display: flex; justify-content: space-between; width: 80%; margin: 0 auto; gap: 20px; align-items: stretch; padding: 0;">

  <!-- Panel 1: Study Area (45%) -->
  <figure style=" flex: 0 0 45%; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; margin: 0;
    border: 1px solid #ccc; border-radius: 5px; padding: 0; /* Removed padding to reduce top/bottom space */  box-sizing: border-box;  position: relative; ">

    <!-- Image wrapper -->
    <div style=" width: 100%; display: flex; justify-content: center;  align-items: center; position: relative;  margin: 0;  padding: 0; ">
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
    <figcaption style=" font-size: 0.9em; font-style: italic; line-height: 1.3; justify-content: center; margin: 2px 0 0 0; /* very small top margin to reduce gap */ padding: 0; ">
        Figure: Geographic locations of study areas across the globe spanning northern and southern hemispheres (United States, a biodiversity hotspot from North America; the Atlantic Forest of Brazil, a biodiversity hotspot, and Paraguay from South America; Holland, the largest tulip bulb producer in the world from Europe; Nepal, a biodiversity hotspot from Asia; urban forests from Africa and Australia) and species (California’s wildflowers, Pleroma, pink trumpet, tulip, rhododendron, and jacaranda) used in the study and spectra of respective flowers. Flowering sample polygons were used to extract flower spectral reflectance across bands corresponding to satellite imagery acquired during the bloom; the number and types of bands (coastal blue [C], blue [B], green [G], red [R], near-infrared [NIR], shortwave infrared 1 [S1], and shortwave infrared 2 [S2]) varied among satellite sensors (SkySat [0.5 m; 4 bands], PlanetScope [3 m; 4 bands], and Landsat [30 m; 7 bands]). Each line shows the mean surface reflectance ± one standard deviation across spectral bands. Dashed, solid, and dotted lines represent SkySat, PlanetScope, and Landsat data.
    </figcaption>

  </figure>

  <!-- Panel 2: Slider (55%) -->
  <figure style=" flex: 0 0 55%; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; margin: 0;
    border: 1px solid #ccc; border-radius: 5px; padding: 0; /* Removed padding to reduce white space */ box-sizing: border-box; ">

    <!-- Slider wrapper -->
    <div style=" flex: 1; display: flex;  justify-content: center;  align-items: center;  width: 100%;  margin: 0;  padding: 0; position: relative; ">
      {% include slider.html
        id="fci"
        before="Jacaranda_RGB.jpg"
        after="Jacaranda_FCI.jpg"
        before_label="RGB Image"
        after_label="Flower Color Index (FCI)"
      %}
    </div>

    <!-- Caption -->
    <figcaption style=" font-size: 0.9em; font-style: italic; line-height: 1.3; margin: 2px 0 0 0; /* reduce space between slider and caption */  padding: 0; ">
        Figure: Visualization of Jacaranda bloom using the Flower Color Index (FCI)-Purple applied to RGB imagery.
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
  Thapa, B., Hardiman, B. S., & Fei, S. (2025). Flower color index for detecting and monitoring warm-colored flowering across scales. <em>International Journal of Applied Earth Observation and Geoinformation</em>, 145, 104978.
  <a href="https://doi.org/10.1016/j.jag.2025.104978" target="_blank" rel="noopener noreferrer">
    DOI
  </a>
</div>


---

## 🌲 Urban Species Mapping Using High-Resolution Multi-Temporal PlanetScope Imagery {#planet}
<div class="project-text-box" style="width: 98%; margin: 0 auto;">
  <p>
    Accurate tree inventories are critical for urban forest management but are challenging to obtain, as many urban trees are located on private property (e.g., backyards) and are therefore excluded from public inventories. Here, we examined the feasibility of tree species identification in a large, heterogeneous urban area (>850 km²) using multi-temporal PlanetScope imagery (3.2 m spatial resolution, multispectral) and inventory data from more than 20,000 ground observations within the <strong>urban forest of the Greater Chicago area</strong>. Our approach achieved an <strong>overall classification accuracy of 0.60 and 0.71 for 18 species and ten genera</strong>, respectively, with accuracies ranging from moderate to high for individual species (0.59–0.92) and genera (0.61–0.91). In particular, we identified <strong>key host tree species</strong> (<em>Fraxinus americana</em>, <em>F. pennsylvanica</em>, and <em>Acer saccharinum</em>) for two damaging invasive insects—<strong>emerald ash borer (EAB, <em>Agrilus planipennis</em>) and Asian longhorn beetle (ALB, <em>Anoplophora glabripennis</em>)</strong>—with accuracies exceeding 0.80. In addition, we demonstrated that including imagery from the <strong>autumn months (September–November)</strong>, either in single-season models or combined multi-season models, improved identification accuracy for <strong>temperate deciduous trees</strong>. Furthermore, the superior classification performance of the support vector machine (SVM) compared to random forest (RF) and neural network (NN) approaches suggests that future work may benefit from evaluating multiple classifiers to identify methods that maximize species-level accuracy. Overall, our study demonstrates the potential of multi-temporal, high-resolution imagery for large-scale urban tree species classification and its applicability to urban forest management.
  </p>
</div>


<!-- Figure Section -->
<div style="display: flex; justify-content: space-between; width: 80%; margin: 0 auto; align-items: stretch; /* stretch panels to equal height */ gap: 20px; min-height: 600px; /* optional: ensures a minimum height */">

  <!-- Left panel: two stacked static images -->
  <div style="flex: 0 0 45%; display: flex; flex-direction: column; justify-content: center; gap: 20px;">

    <!-- Image A -->
    <figure style="margin: 0; text-align: center;">
      <img src="{{ site.baseurl }}/assets/images/MultiTemporal_Imagery.jpg"
           alt="Multi-temporal PlanetScope imagery"
           style="width: 100%; height: auto; border: 1px solid #ccc; border-radius: 5px; object-fit: contain;">
      <figcaption style="font-size: 0.9em; font-style: italic; margin-top: 4px;">
        (a) PlanetScope images capturing leaf phenology.
      </figcaption>
    </figure>

    <!-- Image B -->
    <figure style="margin: 0; text-align: center;">
      <img src="{{ site.baseurl }}/assets/images/TreeSpecies.jpg"
           alt="Urban tree species samples"
           style="width: 100%; height: auto; border: 1px solid #ccc; border-radius: 5px; object-fit: contain;">
      <figcaption style="font-size: 0.9em; font-style: italic; margin-top: 4px;">
        (b) Tree species identification (PlanetScope imagery + LiDAR Crown).
      </figcaption>
    </figure>

  </div>

  <!-- Right panel: two stacked clickable images with zoom hover -->
  <div style="flex: 0 0 50%; display: flex; flex-direction: column; justify-content: center; gap: 20px;">

    <!-- Image C -->
    <figure style="margin: 0; text-align: center; position: relative;">
      <a href="{{ site.baseurl }}/assets/images/Cook_IL_Species.jpg" target="_blank" style="display: block; position: relative; width: 100%;">
        <img src="{{ site.baseurl }}/assets/images/Cook_IL_Species.jpg"
             alt="Tree species distribution in Cook County, Illinois"
             style="display: block; width: 100%; height: auto; border: 1px solid #ccc; border-radius: 5px; object-fit: contain;">
        <span style=" position: absolute; top: 8px; right: 8px;  background: rgba(0,0,0,0.6); color: white; padding: 4px 6px;
          border-radius: 3px; font-size: 1.2em; cursor: pointer; opacity: 0; transition: opacity 0.2s; ">🔍</span>
      </a>
      <figcaption style="font-size: 0.9em; font-style: italic; margin-top: 4px;">
        (c) Urban tree species distribution in Cook County, Illinois.
      </figcaption>
    </figure>

    <!-- Image D -->
    <figure style="margin: 0; text-align: center; position: relative;">
      <a href="{{ site.baseurl }}/assets/images/DuPage_IL_Species.jpg" target="_blank" style="display: block; position: relative; width: 100%;">
        <img src="{{ site.baseurl }}/assets/images/DuPage_IL_Species.jpg"
             alt="Tree species distribution in DuPage County, Illinois"
             style="display: block; width: 100%; height: auto; border: 1px solid #ccc; border-radius: 5px; object-fit: contain;">
        <span style=" position: absolute; top: 8px; right: 8px; background: rgba(0,0,0,0.6); color: white; padding: 4px 6px; border-radius: 3px;
          font-size: 1.2em; cursor: pointer;  opacity: 0;  transition: opacity 0.2s; ">🔍</span>
      </a>
      <figcaption style="font-size: 0.9em; font-style: italic; margin-top: 4px;">
        (d) Urban tree species distribution in DuPage County, Illinois.
      </figcaption>
    </figure>

  </div>

</div>

<!-- Hover effect for zoom icons -->
<style>
  figure a:hover span {
    opacity: 1;
  }
</style>


<!-- Publications Section -->
<h4 class="pub-heading">Publication</h4>
<div class="publication-list">
  Thapa, B.,Daring, L., Choi, D. H., Ardohain, C. M., Firoze, A., Aliaga, D. G., Hardiman, B. S., Fei, S. (2024). Application of multi-temporal satellite iamgery for urban tree species identification. <em>Urban Forestry & Urban Greening</em>, 98, 128409.
  <a href="https://doi.org/10.1016/j.ufug.2024.128409" target="_blank" rel="noopener noreferrer">
    DOI
  </a>
</div>

---

## 🌎 Regional-Scale Species Mapping with Landsat {#landsat}
<div class="project-text-box" style="width: 98%; margin: 0 auto;">
  <p>
    Effective modeling of forest susceptibility to defoliating insect outbreaks requires better understanding of outbreak dynamics, which includes detailed knowledge of the pre- and post-outbreak forest status as well as subsequent feedback mechanisms. In this paper, we strive to fill the forest status need by combining archived Landsat sensor data (pre- and post-outbreak) with different formats and dates of the <strong>U.S. Forest Service’s Forest Inventory and Analysis (FIA) data (periodic [1970s, 1990s] and annual [2003–2006])</strong>. Specifically, we explore the utility of these FIA ground data for calibrating models of forest species and type abundance for mapping past forest composition in the <strong>Border Lakes Ecoregion (BLE)</strong> of the Upper Midwest of the US. Model calibration results between Landsat reflectance and FIA ground data for both total forest basal area and <strong>balsam fir (<em>Abies balsamea</em>)</strong> relative basal area, a preferred <strong>host of the spruce budworm (SBW, <em>Choristoneura fumiferana</em>)</strong>, were poor to moderate (R<sup>2</sup><sub>adj</sub> = 0.39 and 0.48, respectively). Results for <strong>aspen (<em>Populus tremuloides</em>) and spruce (<em>Picea glauca</em> and <em>P. mariana</em>)</strong> abundance yielded substantially better accuracies (R<sup>2</sup><sub>adj</sub> = 0.64 and 0.78; RMSE = 15.56 and 10.65 m<sup>2</sup>·ha<sup>−1</sup>, respectively). Groupings of tree species into broadleaved and conifers substantially improved model calibration results (R<sup>2</sup><sub>adj</sub> range: 0.72–0.91), except for the SBW host group (<em>A. balsamea</em>, <em>P. glauca</em>, and <em>P. mariana</em>). Periodic FIA ground data from the early 1990s generated stronger models compared to other FIA–Landsat date combinations tested. A paired t-test of abundance differences between undisturbed forest from the older 1977 and 1990 periodic inventories was significant (p-value &lt; 0.0001), suggesting possible effects of variable FIA sampling protocol or ground plot positional accuracy through time. However, a similar paired t-test of abundance difference between periodic FIA (1990) and annual FIA (2003–2006) was not significant (p-value = 0.249). We posit four potential factors that may have contributed to weak Landsat–FIA calibration results for species abundance: (1) variation in FIA subplot arrangement and sampling protocols through time, (2) variability in species abundance and heterogeneity among FIA sampling across adjacent Landsat orbital paths, (3) understory species (balsam fir) that are largely hidden from remote detection, and (4) cloud cover and orbital phase mismatches preventing capture of key forest phenology aids. While past and present FIA sampling protocols were not specifically designed for integration with 30-meter satellite sensor data, careful pairing of FIA ground data (past or present) with Landsat sensor data can facilitate reasonable estimates of forest abundance for generalized forest types, and possibly forest species when heterogeneity is low. Nevertheless, we recommend that FIA subplot sampling protocols be augmented to include measurements of forest conditions that are more amenable to integration with 30-meter Landsat sensor data.
  </p>
</div>

<!-- Species distribution text -->
<div style=" width: 80%;  max-width: 1200px;   /* optional: prevents overly wide text on large screens */
  margin: 20px auto;  text-align: left;  color: #555;  font-size: 0.9em;  line-height: 1.5em;
  border: 1px dashed #ccc;  /* temporary to see width, remove later */  padding: 10px;">
  <strong><em>
    Species distribution (total and relative basal area) was mapped for 1985 and 2005. Example outputs are shown below.
  </em></strong>
</div>


   
<div style="width 80%; text-align: left; margin: 20px auto;">
  <strong>
    <em style="color: #555; font-size: 0.8em;">
      Species distribution (total and relative basal area) was mapped for 1985 and 2005. Example outputs are shown below.
    </em>
  </strong>
</div>


<!-- Figure Section -->
<div style="display: flex; justify-content: space-between;  width: 80%; margin: 0 auto; align-items: stretch;  gap: 20px;  min-height: 600px; ">

  <!-- Left panel -->
  <div style="flex: 0 0 60%; display: flex; flex-direction: column; justify-content: center; gap: 20px;">

    <!-- Image C -->
    <figure style="margin: 0; text-align: center; position: relative;">
      <a href="{{ site.baseurl }}/assets/images/SpeciesAbundance_1985.jpg"
         target="_blank"
         style="display: block; position: relative; width: 100%; overflow: hidden;">
        
        <img src="{{ site.baseurl }}/assets/images/SpeciesAbundance_1985.jpg"
             alt="Species distribution"
             class="zoom-img">

        <span class="zoom-icon">🔍</span>
      </a>

      <figcaption style="font-size: 0.9em; font-style: italic; margin-top: 4px;">
        (a) Distribution of species abundance across Minnesota, USA, and adjacent Ontario, Canada, including major protected areas: Superior National Forest, Chippewa National Forest, Voyageurs National Park, and Quetico Provincial Park (Wilderness Class).
      </figcaption>
    </figure>

  </div> <!-- ✅ CLOSE LEFT PANEL -->

  <!-- Right panel -->
  <div style="flex: 0 0 40%; display: flex; flex-direction: column; justify-content: center; gap: 20px;">

    <!-- Image D -->
    <figure style="margin: 0; text-align: center; position: relative;">
      <a href="{{ site.baseurl }}/assets/images/SBW_Host.jpg"
         target="_blank"
         style="display: block; position: relative; width: 100%; overflow: hidden;">
        
        <img src="{{ site.baseurl }}/assets/images/SBW_Host.jpg"
             alt="SBW Host"
             class="zoom-img">

        <span class="zoom-icon">🔍</span>
      </a>

      <figcaption style="font-size: 0.9em; font-style: italic; margin-top: 4px;">
        (b) Distribution of spruce budworm (SBW) host species (balsam fir, white spruce, black spruce) before and after the 1990s outbreak.
      </figcaption>
    </figure>

  </div>

</div>

<!-- Hover & zoom effects -->
<style>
  .zoom-img { display: block; width: 100%; height: auto; border: 1px solid #ccc; border-radius: 5px; object-fit: contain; transition: transform 0.3s ease;}
  figure a:hover .zoom-img {transform: scale(1.05); }

  .zoom-icon { position: absolute; top: 8px;  right: 8px; background: rgba(0,0,0,0.6); color: white; padding: 4px 6px; border-radius: 3px; font-size: 1.2em;
    cursor: pointer; opacity: 0; transition: opacity 0.2s; }

  figure a:hover .zoom-icon {opacity: 1; }
</style>

<!-- Publications Section -->
<h4 class="pub-heading">Publication</h4>
<div class="publication-list">
  Thapa, B., Wolter, P. T., Sturtevant, B. R., & Townsend, P. A. (2020). Reconstructing past forest composition and abundance by using archived Landsat and national forest inventory data. <em>International Journal of Remote Sensing</em>, 41(10), 4022-4056.
  <a href="https://doi.org/10.1080/01431161.2019.1711245" target="_blank" rel="noopener noreferrer">
    DOI
  </a>
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

