# 📊 Bibliometrics — An Interactive Course

A complete, self-contained interactive course on bibliometrics, delivered as a **single HTML file**. 
[![Open in Browser](https://img.shields.io/badge/Open-bibliometrics.html-2563eb?style=for-the-badge&logo=html5)](./bibliometrics.html)

---

## ✨ Features

### 8 Comprehensive Modules
| # | Module | Topics |
|---|--------|--------|
| 1 | Introduction | History, scope, key figures (Garfield, Hirsch, Pritchard), timeline 1917–present |
| 2 | Core Metrics | h-index, g-index, i10-index, Impact Factor, CiteScore, SNIP, SJR |
| 3 | Bibliometric Laws | Lotka's Law, Bradford's Law, Zipf's Law |
| 4 | Network Analysis | Co-citation, bibliographic coupling, co-authorship networks |
| 5 | Database Sources | Web of Science, Scopus, PubMed, Google Scholar, OpenAlex, Dimensions |
| 6 | Science Mapping | VOSviewer-style keyword maps, thematic maps, science cartography |
| 7 | Research Evaluation | REF, ERA, Leiden Ranking, DORA, Leiden Manifesto, CoARA |
| 8 | Limitations & Critiques | Gaming metrics, Matthew Effect, field bias, responsible use |

### Interactive Tools
- **h-index calculator** — paste any citation list, get h-index, g-index, and i10-index with a live bar chart
- **Impact Factor simulator** — enter journal citation/article counts to compute IF with contextual benchmarks
- **Bibliometric law charts** — Lotka, Bradford, and Zipf curves with adjustable sliders (exponent, multiplier, scale)
- **D3.js co-authorship network** — force-directed graph with draggable nodes, hover tooltips, cluster coloring
- **D3.js keyword co-occurrence map** — VOSviewer-style map for a sample bibliometrics corpus
- **Thematic map** — strategic diagram (motor / niche / basic / marginal themes)
- **8 module quizzes** — 32 multiple-choice questions with instant feedback and scoring

### Code Examples
Every module includes:
- **Python code blocks** — using `pandas`, `numpy`, `networkx`, `bibliometrix`-compatible logic
- **R code blocks** — using the `bibliometrix` package, `igraph`, `openalexR`
- **In-browser Python runner** — powered by [Pyodide](https://pyodide.org), runs real Python (with `numpy` + `pandas`) directly in the browser, no installation needed
- **Copy-to-clipboard** button on every code block
- **Syntax highlighting** via highlight.js

### UX
- Sidebar navigation with progress tracking
- Module completion buttons
- Smooth transitions and animations
- Responsive layout (desktop + tablet)

---

## 🚀 Getting Started

**No installation required.** Just download and open:

```bash
git clone https://github.com/sandwidinarcisse/Bibliometrie.git
cd Bibliometrie
# Then open bibliometrics.html in any modern browser
```

Or [download the HTML file directly](./bibliometrics.html) and double-click it.

> **Note on the Python runner:** The first time you click ▶ Run on any code block, Pyodide (~10 MB) and the numpy/pandas packages are downloaded from a CDN. This takes 15–30 seconds on the first run. Subsequent runs in the same session are instant.

---

## 🛠️ Tech Stack

| Library | Purpose | Source |
|---------|---------|--------|
| [D3.js v7](https://d3js.org) | Force-directed network graphs | CDN |
| [Chart.js v4](https://chartjs.org) | Lotka/Bradford/Zipf/Thematic charts | CDN |
| [Pyodide v0.24](https://pyodide.org) | In-browser Python execution | CDN |
| [highlight.js v11](https://highlightjs.org) | Code syntax highlighting | CDN |
| Google Fonts (Inter, JetBrains Mono) | Typography | CDN |

Everything else — layout, navigation, quizzes, calculators — is vanilla HTML/CSS/JavaScript with no framework.

---

## 📁 Repository Structure

```
Bibliometrie/
└── bibliometrics.html    # The entire course — single self-contained file
└── README.md             # This file
```

---

## 📚 Course Content Overview

### Bibliometric Laws (Module 3)
The three empirical laws of bibliometrics, each with an interactive chart:

- **Lotka's Law** `f(n) = C / nᵅ` — inverse square law of author productivity
- **Bradford's Law** `n₁ : n₂ : n₃ = 1 : k : k²` — scattering of journal literature
- **Zipf's Law** `f(r) ∝ 1/rˢ` — power-law word/citation frequency distribution

### Key Metrics (Module 2)
```
h-index   = largest h where h papers each have ≥ h citations
g-index   = largest g where top-g papers together have ≥ g² citations
IF(year)  = citations in Y to (Y-1 and Y-2) / citable articles in (Y-1 and Y-2)
FWCI      = paper citations / expected citations for field+year+type
```

### Database Comparison (Module 5)
| Database | Records | Cost | Citation Data | API |
|----------|---------|------|--------------|-----|
| Web of Science | ~21K journals | Paid | ✅ | ✅ (InCites) |
| Scopus | ~27K journals | Paid | ✅ | ✅ |
| PubMed | ~35M records | Free | ❌ | ✅ |
| Google Scholar | ~200M+ | Free | ✅ | ❌ |
| OpenAlex | ~250M works | Free | ✅ | ✅ (open) |

---

## 🎓 Learning Outcomes

After completing this course, you will be able to:

- Compute and interpret h-index, g-index, Impact Factor, CiteScore, and field-normalized indicators
- Apply Lotka's, Bradford's, and Zipf's laws to real literature datasets
- Build and analyze co-authorship and co-citation networks using Python and R
- Select the appropriate bibliographic database for a given research task
- Create science maps (keyword co-occurrence, thematic maps) using VOSviewer or bibliometrix
- Critically evaluate the limitations and misuse potential of bibliometric indicators
- Apply responsible metrics principles (DORA, Leiden Manifesto, CoARA)

---

## 🤝 Contributing

Contributions are welcome. Potential improvements:

- Add more Pyodide-runnable examples (e.g., live OpenAlex API calls)
- Extend the network module with real dataset examples
- Add a module on altmetrics and open science indicators
- Translate to French, Spanish, or Portuguese

Please open an issue or submit a pull request.

---

## 📄 License

This project is released under the [MIT License](LICENSE).

---

## 📖 Key References

- Pritchard, A. (1969). Statistical bibliography or bibliometrics? *Journal of Documentation*, 25(4), 348–349.
- Hirsch, J. E. (2005). An index to quantify an individual's scientific research output. *PNAS*, 102(46), 16569–16572.
- Garfield, E. (1955). Citation indexes for science. *Science*, 122(3159), 108–111.
- Hicks, D., Wouters, P., Waltman, L., de Rijcke, S., & Rafols, I. (2015). The Leiden Manifesto for research metrics. *Nature*, 520, 429–431.
- Aria, M., & Cuccurullo, C. (2017). bibliometrix: An R-tool for comprehensive science mapping analysis. *Journal of Informetrics*, 11(4), 959–975.
- van Eck, N.J., & Waltman, L. (2010). Software survey: VOSviewer, a computer program for bibliometric mapping. *Scientometrics*, 84(2), 523–538.

---

*Built with ❤️ for researchers, librarians, and research evaluators.*
