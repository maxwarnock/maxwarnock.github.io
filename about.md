---
layout: default
title: About Me
show_profile: true
permalink: /about/
---
<style>
.about-row {
  display: flex;
  align-items: flex-start;
  gap: 20px;
  flex-wrap: wrap;
  margin: 20px 0 0 20px;
}

.about-card {
  flex: 0 1 650px;
  min-width: 0;
  box-sizing: border-box;
  font-size: 16px;
  background: rgba(255, 255, 255, 0.10);
  color: white;
  padding: 24px;
  border-radius: 8px;
  box-shadow: 0 4px 11px rgba(0,0,0,0.20);
}

.about-card p {
  margin: 0 0 1em 0;
}

.about-card p:last-child {
  margin-bottom: 0;
}

.about-photo-wrap {
  flex: 1 1 240px;
  display: flex;
  justify-content: center;
  padding-top: 0.75in;
  margin-right: -20px;
}

.about-photo {
  width: 220px;
  max-width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.30);
}

@media (max-width: 1200px) {
  .about-photo-wrap {
    justify-content: flex-start;
    padding-top: 0;
    margin-right: 0;
  }
}
</style>

<div class="about-row">
<div class="about-card">
<p>I'm an early-career GIS analyst interested in environmental research using GIS and Earth data to answer questions for topics ranging from urban planning and land management, to ecosystem health, soils, hydrology, species migration, and more. I recently completed a B.A. in Geography from the University of Colorado Boulder and a graduate certificate in Earth Data Analytics from CU's Earth Lab.</p>

<p>My recent work ranges from custom Python tools to web maps and StoryMaps that make spatial analysis easy for anyone to explore. With a small team, I built an algorithm and web tool that identifies land swaps to consolidate ownership around the Pawnee National Grassland. The tool identified nearly 700 swap proposals that consolidate land ownership while benefitting both private and government stakeholders. The top ranked proposals add nearly 14,500 acres to a single contiguous patch. The tool is currently being considered for state-wide use in Colorado with the U.S. Forest Service in partnership with the non-profit Grasslands Unlimited. 
</p>

<p>I also built an automated tool for mapping the Wildland-Urban Interface (WUI) that matched the widely used SILVIS Lab WUI maps with up to 97% accuracy. The tool streamlines data download and processing, allowing users to create WUI maps for the past 25 years. On the remote sensing side, I've measured glacial retreat in the Swiss Alps and Grand Teton National Park using decades of satellite imagery. As a volunteer GIS Technician for the Salvation Army, I built ArcGIS Online maps that help people find services near them, and I automated the team's mapping workflows with ArcPy.</p>

<p>Outside of GIS and geography, I'm a classically trained pianist and teach piano part-time in Boulder. In my free time I enjoy enjoy hiking and spending time in nature with friends and family. 
</p>
</div>
<div class="about-photo-wrap"><img class="about-photo" src="/img/at_glacier.png" alt="Mountain lake in Rocky Mountain National Park"></div>
</div>
