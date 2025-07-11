## GreenSentinel-AI

GreenSentinel AI: Monitoring Illegal Land Use with Satellite Imagery and Text Analysis
*Final project for the Building AI course*

## Summary

GreenSentinel AI is an intelligent environmental monitoring tool that uses satellite image comparison and NLP analysis of environmental reports to detect deforestation, land encroachment, and illegal activities. It empowers decision-makers in developing countries with AI-driven alerts and visualizations.

## Background

Environmental violations like illegal construction and deforestation are major issues in developing countries due to lack of monitoring tools and slow bureaucratic response. I personally care about climate justice and have worked on a similar AI project before. This solution aims to support local governments with smart alerts and clear evidence.

Problems this idea addresses:

* Unmonitored deforestation and land misuse
* Slow detection of illegal environmental activities
* Lack of automated, low-cost monitoring systems in resource-constrained areas

## How is it used?

The system is used by:

* Environmental ministries
* Local municipalities
* NGOs working in conservation

Workflow:

1. Upload two satellite images of the same location from different dates
2. Upload a local report or article related to the area
3. The system detects land changes in images using computer vision (OpenCV + edge detection or segmentation)
4. Texts are summarized and analyzed using a lightweight LLM (like Gemma 3n or DistilBERT) for environmental keywords
5. Generates an alert report with map visuals, analysis, and suggested actions

<img src="https://upload.wikimedia.org/wikipedia/commons/2/22/DeforestationNASA.jpg" width="400">

## Data sources and AI methods

Data:

* Sentinel-2 satellite imagery (Copernicus EU)
* Public reports, government PDFs, or scraped news from affected regions

AI techniques:

* Image change detection (difference + thresholding)
* NLP text summarization and keyword extraction
* Lightweight transformer model or open-source LLM (Gemma 3n)

## Challenges

* May not detect slow or small changes in low-resolution images
* Text data may be biased or not up-to-date
* Requires access to cloud-free satellite data
* Cannot enforce law, only assist decision-making

## What next?

* Add real-time alerting with APIs
* Build a public dashboard with interactive maps
* Train a custom model on deforestation datasets
* Integrate drone footage in future versions
* Collaborate with local authorities in test regions (e.g., Egypt, Kenya, Brazil)

## Acknowledgments

* Satellite data from [Copernicus EU](https://scihub.copernicus.eu/)
* NLP techniques inspired by [Hugging Face Transformers](https://huggingface.co/transformers/)
* Markdown formatting help from Building AI course template

> *This is a Building AI course project by Ibrahim Hafez, GitHub: [github.com/ibrahimhafez](https://github.com/Ebrahimhafiz)*
