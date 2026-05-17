# Practical Data Analysis – Learning Guide

An interactive, self-contained learning guide for practical data science and machine learning, delivered as a single HTML file — no installation required.

## Demo

Open `ds.html` directly in any modern browser. Nothing to install, no server needed.

## Overview

This guide walks through 14 chapters of hands-on data analysis, from loading your first CSV to building classifiers and simulating financial models. Each chapter includes:

- **Overview** — concept explanations with examples and diagrams
- **Exercises** — practice problems to test your understanding
- **Solutions** — worked answers with explanations
- **Code** — ready-to-run Python scripts you can copy and execute locally

## Chapters

| # | Title | Topics |
|---|-------|--------|
| 1 | Getting Started with Data Analysis | Python basics, exploratory data analysis, pandas intro |
| 2 | Working with Data | Data loading, cleaning, merging, CSV/Excel handling |
| 3 | Data Visualization | matplotlib, seaborn, chart types, Anscombe's quartet |
| 4 | Text Classification | Naive Bayes, spam detection, bag-of-words, confusion matrix |
| 5 | Image Similarity | Dynamic Time Warping, color histograms, similarity-based retrieval |
| 6 | Stock Simulation | Random walks, Geometric Brownian Motion, Monte Carlo simulation |
| 7 | Gold Price Analysis | Time series regression, feature engineering, forecasting |
| 8 | Support Vector Machines | SVMs, kernels, classification boundaries |
| 9 | Disease Modeling | Epidemiological models (SIR), simulation, curve fitting |
| 10 | Social Network Analysis | Graph theory, NetworkX, centrality, community detection |
| 11 | Sentiment Analysis | NLP, lexicon-based scoring, VADER, opinion mining |
| 12 | MongoDB & NoSQL | Document databases, queries, aggregation pipelines |
| 13 | MapReduce & Big Data | Distributed computing concepts, Hadoop-style patterns |
| 14 | Pandas & Jupyter Deep Dive | Advanced pandas, indexing, performance, Jupyter tips |

## Features

- **No dependencies** — single `.html` file, works offline
- **Progress tracking** — chapters are marked complete as you work through them; a progress bar updates in the sidebar
- **Search** — filter chapters by keyword from the sidebar
- **Dark / Light mode** — toggle in the top bar
- **Responsive** — works on desktop and mobile browsers
- **Copy-ready code** — Python snippets in each chapter can be copied and run in your local environment

## Usage

```bash
# Clone the repo
git clone https://github.com/your-username/your-repo.git

# Open the guide
open ds.html          # macOS
start ds.html         # Windows
xdg-open ds.html      # Linux
```

Or simply drag `ds.html` into your browser.

## Running the Code Examples

The code snippets in each chapter require Python 3.8+ and the following libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy networkx pymongo
```

Each chapter's **Code** tab contains a self-contained Python script. Copy it into a `.py` file or paste it into a Jupyter notebook and run it directly.

## Browser Compatibility

Works in all modern browsers:

- Chrome / Edge 90+
- Firefox 88+
- Safari 14+

## License

MIT — free to use, share, and adapt.
