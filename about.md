---
layout: default
title: About Me
show_profile: true
permalink: /about/
---
<style>
.collage {
  box-sizing: border-box;
  width: 650px;
  max-width: 100%;
  margin: 20px 0 40px 56px;
  padding: 14px 0;
  background: rgba(255, 255, 255, 0.10);
  border-radius: 8px;
  box-shadow: 0 4px 11px rgba(0, 0, 0, 0.20);
}

.c-card {
  position: relative;
  box-sizing: border-box;
  padding: 26px 170px 26px 28px;
  min-height: 200px;
  font-family: "Segoe UI", system-ui, -apple-system, Roboto, "Helvetica Neue", sans-serif;
  font-size: 16px;
  line-height: 1.7;
  letter-spacing: 0.01em;
  color: #d8d4cc;
}

.c-card p {
  margin: 0;
}

.c-photo {
  position: absolute;
  top: 50%;
  right: -110px;
  width: 240px;
  height: auto;
  border: 6px solid #fff;
  border-radius: 4px;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.45);
  transform: translateY(-50%) rotate(var(--rot, 3deg));
}

.c-card:nth-child(2) .c-photo { --rot: -3deg; }
.c-card:nth-child(3) .c-photo { --rot: 2deg; width: 200px; }
.c-card:nth-child(4) .c-photo { --rot: -2deg; }

@media (max-width: 1100px) {
  .c-card { padding: 24px; min-height: 0; }
  .c-photo {
    position: static;
    display: block;
    margin: 16px auto 0;
    transform: rotate(var(--rot, 2deg));
    right: auto;
  }
}

@media (max-width: 768px) {
  .collage { margin-left: 20px; }
}
</style>

<div class="collage">
<div class="c-card">
<p>I'm an early-career GIS analyst interested in environmental planning and earth science, using spatial data and remote sensing to understand how communities and landscapes change. I recently completed a B.A. in Geography from the University of Colorado Boulder and a graduate certificate in Earth Data Analytics from CU's Earth Lab.</p>
<img class="c-photo" src="/img/at_glacier.jpg" alt="Max at a glacier-fed lake in Rocky Mountain National Park">
</div>
<div class="c-card">
<p>My recent work ranges from custom Python tools to web maps and StoryMaps that make spatial analysis easy for anyone to explore. With a small team, I built an algorithm and web tool that identifies land swaps to consolidate ownership around the Pawnee National Grassland. The tool identified nearly 700 swap proposals that consolidate land ownership while benefitting both private and government stakeholders. The top ranked proposals add nearly 14,500 acres to a single contiguous patch. The tool is currently being considered for state-wide use in Colorado with the U.S. Forest Service in partnership with the non-profit Grasslands Unlimited.</p>
<img class="c-photo" src="/img/pawnee_cover.png" alt="Pawnee National Grassland land swap map">
</div>
<div class="c-card">
<p>I also built an automated tool for mapping the wildland-urban interface that matched the widely used SILVIS Lab WUI maps with up to 97% accuracy. On the remote sensing side, I've measured glacial retreat in the Swiss Alps and Grand Teton National Park using decades of satellite imagery. As a volunteer GIS Technician for the Salvation Army, I built ArcGIS Online maps that help people find services near them, and I automated the team's mapping workflows with ArcPy.</p>
<img class="c-photo" src="/img/wui_cover.png" alt="Wildland-urban interface map of Colorado">
</div>
<div class="c-card">
<p>I'm most interested in two areas: GIS for city and regional planning, and remote sensing for monitoring environmental change. Outside of GIS and geography, I'm a classically trained pianist and teach piano part-time in Boulder.</p>
<img class="c-photo" src="/img/about_photo.jpg" alt="Mountain lake in Rocky Mountain National Park">
</div>
</div>
