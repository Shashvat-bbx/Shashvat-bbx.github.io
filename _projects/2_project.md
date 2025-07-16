---
layout: page
title: Manim Educational Video Generator
description: Agentic Manim Video Pipeline for Automated Educational Content
img: assets/img/Manim_project_images/Manim_project_thumbnail.png
importance: 2
category: fun
related_publications: true
---

The **Manim Educational Video Generator** is an agentic project designed to automate the creation of educational videos using AI agents, Manim, and video post-processing tools. 

Given a video topic, a planning agent structures the content into multiple scenes. For each scene, Manim code is generated in parallel. Once all scenes are rendered as individual video clips, they are concatenated into a complete educational video using **FFmpeg**.

### Flowchart
<div class="row justify-content-center">
  <div class="col-sm-4"></div>
  <div class="col-sm-4 d-flex justify-content-center">
    {% include figure.liquid loading="eager" path="assets/img/Manim_project_images/Manim_project_flowchart.png" title="Video Concatenation Pipeline" class="img-fluid rounded z-depth-1" style="max-width: 250px;" %}
  </div>
  <div class="col-sm-4"></div>
</div>
---

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/Manim_project_images/Scene_planner.png" title="Planning Agent in Action" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/Manim_project_images/Scene_generation.png" title="Scene Code Generation" class="img-fluid rounded z-depth-1" %}
  </div>
  
</div>

<div class="caption">
  Left: AI agent structures scenes. Middle: Manim renders each scene. Right: FFmpeg joins scenes into one final video.
</div>

### How It Works:

- **Step 1:** Topic input triggers the planning agent.
- **Step 2:** Planning agent breaks down the topic into scenes.
- **Step 3:** Scene-wise Manim code is auto-generated and rendered in parallel.
- **Step 4:** Individual scene videos are stitched together using FFmpeg.

---
### Sample Output Scene Generated
<div class="row justify-content-center">
  <div class="col-sm-3"></div>
    <video controls class="img-fluid rounded z-depth-1">
        <source src="/assets/video/Manim_output_video.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
  
  <div class="col-sm-3"></div>
</div>



---

### Limitations & Challenges:

- Minor bugs in some scene code occasionally affect the final video rendering pipeline.
- Future improvement: Integrating Text-to-Speech (TTS) models to add voice narration.  
  **Challenge:** Syncing audio duration exactly with scene length during Manim rendering.

---

_The project aims to combine structured AI-driven planning, mathematical animation, and video processing pipelines into an end-to-end educational content generator._  
