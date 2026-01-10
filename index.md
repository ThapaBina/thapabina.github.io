---
layout: default
title: Home
---

<style>
  .profile-container {
    display: flex;
    align-items: flex-start;
    gap: 30px;
    flex-wrap: wrap;
    max-width: 900px;
    margin: 40px auto;
  }

  .profile-image {
    flex: 0 0 200px;
  }

  .profile-image img {
    width: 200px;
    border-radius: 8px;
  }

  .profile-text {
    flex: 1;
    min-width: 300px;
  }

  .tabs {
    max-width: 900px;
    margin: 40px auto 0 auto;
    display: flex;
    gap: 20px;
  }

  .tabs a {
    padding: 10px 20px;
    text-decoration: none;
    background-color: #0366d6;
    color: white;
    border-radius: 5px;
    font-weight: 600;
  }

  .tabs a:hover {
    background-color: #024ea2;
  }
</style>

<div class="profile-container">
  <div class="profile-image">
    <img src="/assets/images/BinaThapa_Profile.jpg" alt="Bina Thapa Profile Picture" />
  </div>

  <div class="profile-text">
    <p class="profile-name">Bina Thapa </p>
    <p>
      I am a <strong>postdoctoral researcher at Purdue University</strong> specializing in the remote sensing of forested ecosystems.
      My research utilizes multispectral, hyperspectral, and LiDAR data to investigate forest ecosystem patterns and processes, including species identification, phenology monitoring, and disturbance assessment.
    </p>

    <p>
      I aim to advance our understanding of forest ecosystem dynamics and to develop methods that enhance forest monitoring and characterization.
    </p>

    <p>
      Currently, I am working under the supervision of
      <a href="https://web.ics.purdue.edu/~sfei/feiS.php" target="_blank">Dr. Songlin Fei</a> and
      <a href="https://www.purdue.edu/fnr/sites/hardiman/" target="_blank">Dr. Brady S. Hardiman</a>.
    </p>

    <p>
      <strong>Research Focus:</strong> Species identification, phenology monitoring, disturbance assessment<br />
      <strong>Methodologies:</strong> Multispectral, hyperspectral, LiDAR analysis, algorithm development
    </p>
  </div>
</div>

<div class="tabs">
  <a href="/research/">Research</a>
  <a href="/teaching/">Teaching</a>
  <a href="https://scholar.google.com/citations?user=s5t-GKgAAAAJ&hl=en" target="_blank">Google Scholar</a>
</div>
