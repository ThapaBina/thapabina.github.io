---
layout: default
title: Home
---

<style>
/* Container for photo + text */
.profile-container {
  display: flex;
  align-items: center; /* vertical alignment */
  gap: 30px;
  flex-wrap: wrap;
  max-width: 900px;
  margin: 40px auto;
}

/* Profile image */
.profile-image {
  flex: 0 0 200px;
}

.profile-image img {
  width: 200px;
  border-radius: 8px;
}

/* Text next to image */
.profile-text {
  flex: 1;
  min-width: 300px;
  margin-top:0; /*remove any top margin */
}

/* Name styling */
.profile-name {
  font-size: 2.0em;  /* bigger font */
  font-weight: bold;
  margin-bottom: 15px;
}

/* Bottom tabs */
.tabs {
  max-width: 900px;
  margin: 40px auto 0 auto;
  display: flex;
  gap: 20px;
}

.tabs a {
  padding: 8px 15px;        /*smaller tabs */
  text-decoration: none;
  background-color: #36352e;   /*black background */
  color: #f1e5ab;               /*gold text */
  border-radius: 5px;
  font-weight: 600;
}

.tabs a:hover {
  background-color: #333333;   /* slightly lighter black on hover */
  color: #FFD700;              /* bright gold on hover */
}

</style>

<div class="profile-container">
  <!-- Left: profile photo -->
  <div class="profile-image">
    <img src="/assets/images/BinaThapa_Profile.jpg" alt="Bina Thapa Profile Picture" />
  </div>

  <!-- Right: text content -->
  <div class="profile-text">
    <p class="profile-name">Bina Thapa</p>

    <p>
      I am a postdoctoral researcher at Purdue University specializing in the remote sensing of forested ecosystems.
      My research utilizes multispectral, hyperspectral, and LiDAR data to investigate forest ecosystem patterns and processes, including species identification, phenology monitoring, and disturbance assessment.
    </p>

    <p>
      I aim to advance our understanding of forest ecosystem dynamics and to develop methods that enhance forest monitoring and characterization.
    </p>

    <p>
      <strong>Research Focus:</strong> Species identification, phenology monitoring, disturbance assessment<br />
      <strong>Methodologies:</strong> Multispectral, hyperspectral, LiDAR analysis, algorithm development
    </p>
  </div>
</div>

<!-- Bottom tabs -->
<div class="tabs">
  <a href="/research/">Research</a>
  <a href="/teaching/">Teaching</a>
  <a href="https://scholar.google.com/citations?user=s5t-GKgAAAAJ&hl=en" target="_blank">Google Scholar</a>
</div>
