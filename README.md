# FDH-G8
GitHub repository for Group 8 in Foundations of Digital Humanities 2023.

# Project README

## Introduction

"**Hadji in Syria: or, Three years in Jerusalem**" by Sarah Barclay Johnson (1858) serves as the cornerstone for this digital humanities project. The aim is to create a digital map of the toponyms found in Johnson's 19th-century exploration of Jerusalem, linking historical narrative to modern geography. The project blends literature, history, and technology to offer a dynamic resource for both scholars and enthusiasts, enhancing the understanding of Jerusalem's historical landscape.

## Deliverables

- A pre-processed textual dataset from the book.
- Results from Named Entity Recognition (NER) via Spacy and GPT-4.
- A report comparing NER effectiveness between Spacy and GPT-4.
- A manually labeled dataset for NER validation on a chapter.
- Scripts for automating Wikipedia searches and location data extraction.
- A dataset with coordinates for identified locations.
- GeoPandas mapping files for visualizing named locations.
- Narrative journey maps with highlighted locations and paths.
- A platform showcasing project outputs and interactive maps.

## Methodologies

### Text Preparation

The project began with OCR text acquisition from Google Books, followed by a quality assessment using the NLTK library. Preprocessing was tailored specifically for this project, preserving the text's original structure.

### Location Detection

#### Spacy's NER

Initial NER was conducted using Spacy's pre-trained models, aiming to extract toponyms tagged as "GPE" and "LOC". Challenges included significant mislabeling due to the historical nature of the content.

#### GPT-4's NER

Following Spacy, GPT-4 was tested for its NER capabilities, focusing on chronological location extraction and interaction details, formatted in JSON. Despite initial challenges, GPT-4 provided a more specific and comprehensive toponym list.

#### Manual Analysis and Model Selection

A detailed manual detection of locations in Chapter 3 was performed, resulting in a foundational dataset cross-referenced with Wikipedia for accuracy.

### Data Visualization and Platform Development

The final phase involved mapping the author's route using GeoPandas and visualizing it with Plotly and Mapbox. A dedicated website was created to display the interactive maps, providing a user-friendly interface for exploring the project's findings.
