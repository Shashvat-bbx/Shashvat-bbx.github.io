---
layout: page
title: DTU_Bot — Intelligent PDF Query System for DTU
description: Smart India Hackathon-Style AI System for DTU Academic Document Queries
img: assets/img/DTU_bot_thumbnail.png
importance: 2
category: work
related_publications: true
---

### DTU_Bot — Intelligent PDF Query System for DTU

An end-to-end AI-powered system for scraping, parsing, and conversational querying of official notices, syllabi, and documents from **Delhi Technological University (DTU)**.

---

### Key Features:

- **Automated Scraping:**  
  Extracts PDF links from DTU’s official notices and pages.

- **Bulk Downloading & Metadata Mapping:**  
  Downloads PDFs and tracks their sources.

- **OCR & Parsing:**  
  Extracts text from both text-based and image-based PDFs.

- **Vector Store for Semantic Search:**  
  Embeds documents using HuggingFace models with FAISS indexing.

- **Conversational RAG QA:**  
  Users can query DTU documents using natural language and receive context-rich, cited answers powered by LLMs.

- **Modular Pipeline Design:**  
  Each system stage is a separate, reusable component.

---

### Project Flowchart


<div class="row justify-content-center">
  <div class="col-sm-4"></div>
  <div class="col-sm-4 d-flex justify-content-center">
    {% include figure.liquid loading="eager" path="assets/img/DTU_bot_flowchart.png" title="Project Flowchart" class="img-fluid rounded z-depth-1" style="max-width: 250px;" %}
  </div>
  <div class="col-sm-4"></div>
</div>
<div class="caption">
  Left: Automated PDF Scraping. Middle: OCR Pipeline. Right: Live Conversational QA.
</div>

---

### System Workflow:

- **Step 1:** Scrape PDF links from official web pages.
- **Step 2:** Download PDFs and map metadata.
- **Step 3:** Perform OCR and text extraction.
- **Step 4:** Embed extracted content into a vector store.
- **Step 5:** Enable real-time conversational querying using LLM-powered RAG.

---

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    <video controls class="img-fluid rounded z-depth-1">
      <source src="/assets/video/DTU_bot_demo.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

<div class="caption">
  Live demo of DTU_Bot querying DTU academic documents.
</div>

---

_This project brings together web scraping, computer vision, vector search, and large language models into a single intelligent academic assistant for Delhi Technological University._
