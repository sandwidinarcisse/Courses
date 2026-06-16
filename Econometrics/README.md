# Introductory Econometrics — Interactive Learning Guide

A self-contained, browser-based study companion for introductory econometrics, aligned with Wooldridge's *Introductory Econometrics: A Modern Approach*.

## Overview

`econometrics.html` is a single-file interactive guide covering 19 chapters of applied econometrics. No installation, server, or internet connection required — just open the file in any modern browser.

## Contents

The guide spans three difficulty tiers across 19 chapters:

**Beginner (Ch. 1–4)**
- Ch. 1 — The Nature of Econometrics and Economic Data
- Ch. 2 — The Simple Regression Model
- Ch. 3 — Multiple Regression Analysis: Estimation
- Ch. 4 — Multiple Regression Analysis: Inference

**Intermediate (Ch. 5–12)**
- Ch. 5 — Multiple Regression Analysis: OLS Asymptotics
- Ch. 6 — Multiple Regression Analysis: Further Issues
- Ch. 7 — Dummy Variables (Binary/Qualitative Variables)
- Ch. 8 — Heteroskedasticity
- Ch. 9 — More on Specification and Data Issues
- Ch. 10 — Basic Regression Analysis with Time Series Data
- Ch. 11 — Further Issues in Using OLS with Time Series Data
- Ch. 12 — Serial Correlation and Heteroskedasticity in Time Series

**Advanced (Ch. 13–19)**
- Ch. 13 — Pooling Cross Sections & Simple Panel Data Methods
- Ch. 14 — Advanced Panel Data Methods
- Ch. 15 — Instrumental Variables and Two Stage Least Squares
- Ch. 16 — Simultaneous Equations Models
- Ch. 17 — Limited Dependent Variable Models
- Ch. 18 — Advanced Time Series Topics
- Ch. 19 — Carrying Out an Empirical Project

## Features

- **Progress tracking** — chapters marked complete are saved in your browser across sessions
- **Search** — filter chapters by keyword from the sidebar
- **Tabbed chapter view** — each chapter has Overview, Exercises, Solutions, and Python starter code tabs
- **Collapsible solutions** — attempt exercises before revealing answers
- **Learning paths** — six curated paths (Complete Beginner, Intermediate Track, Advanced Methods, Time Series Focus, Causal Inference, Project Ready)
- **Dark/light mode** — toggle via the topbar
- **Fully offline** — no external dependencies; works without an internet connection

## Usage

1. Download or clone this repository.
2. Open `econometrics.html` in any modern browser (Chrome, Firefox, Edge, Safari).
3. Use the sidebar to navigate chapters or select a learning path from the home page.
4. Work through the exercises, check solutions, and copy the Python starter code into your own environment.

## Python Code

Each chapter includes an `activities.py` starter file with template code for that chapter's exercises. Copy the code from the **Code** tab into a local `.py` file or Jupyter notebook. You will need:

```
pip install numpy pandas statsmodels matplotlib scipy
```

## Reference

Based on:
> Wooldridge, J. M. (2020). *Introductory Econometrics: A Modern Approach* (7th ed.). Cengage Learning.
