---
layout: default
title: About Me
show_profile: true
permalink: /about/
---
<style>
.about-card {
  display: flex;
  align-items: flex-start;
  gap: 28px;
  flex-wrap: wrap;
  max-width: 1000px;
  margin: 20px 0 0 20px;
  font-size: 16px;
  background: rgba(255, 255, 255, 0.10);
  color: white;
  padding: 24px;
  border-radius: 8px;
  box-shadow: 0 4px 11px rgba(0,0,0,0.20);
}

.about-text {
  flex: 1 1 380px;
  min-width: 0;
}

.about-text p {
  margin: 0 0 1em 0;
}

.about-text p:last-child {
  margin-bottom: 0;
}

.about-photo {
  flex: 0 1 340px;
  max-width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.30);
}
</style>

<div class="about-card">
<div class="about-text">
<p>I'm an early-career GIS analyst interested in environmental planning and earth science, using spatial data and remote sensing to understand how communities and landscapes change. I recently completed a B.A. in Geography from the University of Colorado Boulder and a graduate certificate in Earth Data Analytics from CU's Earth Lab.</p>

<p>My recent work ranges from custom Python tools to web maps and StoryMaps that make spatial analysis easy for anyone to explore. With a small team, I built an algorithm and web tool that identifies land swaps to consolidate ownership around the Pawnee National Grassland. The tool identified nearly 700 swap proposals that consolidate land ownership while benefitting both private and government stakeholders. The top ranked proposals add nearly 14,500 acres to a single contiguous patch. The tool is currently being considered for state-wide use in Colorado with the U.S. Forest Service in partnership with the non-profit Grasslands Unlimited.</p>

<p>I also built an automated tool for mapping the wildland-urban interface that matched the widely used SILVIS Lab WUI maps with up to 97% accuracy. On the remote sensing side, I've measured glacial retreat in the Swiss Alps and Grand Teton National Park using decades of satellite imagery. As a volunteer GIS Technician for the Salvation Army, I built ArcGIS Online maps that help people find services near them, and I automated the team's mapping workflows with ArcPy.</p>

<p>I'm most interested in two areas: GIS for city and regional planning, and remote sensing for monitoring environmental change. Outside of GIS and geography, I'm a classically trained pianist and teach piano part-time in Boulder.</p>
</div>
<img class="about-photo" src="/img/about_photo.jpg" alt="Mountain lake in Rocky Mountain National Park">
</div>
