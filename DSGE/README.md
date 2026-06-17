# DSGE Models: An Interactive Graduate Course

A single-file, self-contained interactive course on Dynamic Stochastic General Equilibrium (DSGE) models — from foundational concepts to frontier research. Open `dsge.html` directly in any modern browser. No server, no build tools, no installation required.

## Contents

The course covers ten progressive modules:

1. **Introduction** — What DSGE models are, their history (Kydland-Prescott 1982 → Smets-Wouters 2007 → HANK), and why they matter
2. **Households** — Utility maximization, Euler equation, labor supply, budget constraint
3. **Firms & Pricing** — Dixit-Stiglitz aggregation, Calvo staggered pricing, New Keynesian Phillips Curve derivation
4. **Monetary & Fiscal Policy** — Taylor rule, Taylor principle, government budget constraint, fiscal multipliers
5. **Key Equations & Log-Linearization** — The three-equation NK system, log-linearization technique, natural rate of interest
6. **Interactive IRF Simulation** — Real-time impulse response explorer (see below)
7. **Solution Methods** — Blanchard-Kahn conditions, state-space representation, perturbation methods (1st and 2nd order)
8. **Bayesian Estimation** — Prior distributions, Kalman filter likelihood, Metropolis-Hastings MCMC, identification
9. **Advanced Topics** — Heterogeneous agents (Aiyagari), financial frictions (BGG accelerator), ZLB, open-economy DSGE, HANK models
10. **Final Assessment** — 10-question comprehensive exam with instant graded feedback

## Interactive Features

### IRF Simulator
Adjust model parameters via sliders and see impulse response functions update in real time (powered by Plotly.js):
- **Shocks:** Monetary policy, demand, cost-push
- **Parameters:** β (discount factor), σ (inverse IES), θ (Calvo), φ_π and φ_y (Taylor rule coefficients), ρ (shock persistence)
- **Variables plotted:** Output gap, inflation (annualized), nominal rate, real rate

### Code Examples
Every module includes annotated Python and R code with:
- One-click copy to clipboard
- **Run in Browser** button for Python snippets (via Pyodide WebAssembly — no local installation needed)

### Quizzes & Glossary
- Self-check quizzes with instant feedback at the end of each module
- 32-term glossary accessible from any section, with search

## Usage

```bash
git clone https://github.com/your-username/dsge-course.git
cd dsge-course
open dsge.html        # macOS
start dsge.html       # Windows
xdg-open dsge.html   # Linux
```

Or simply download `dsge.html` and open it in Chrome, Firefox, Edge, or Safari.

**On first load**, the page fetches the following CDN resources (internet required):
- [MathJax 3](https://cdn.jsdelivr.net/npm/mathjax@3/) — LaTeX equation rendering
- [Plotly.js 2.26](https://cdn.plot.ly/) — Interactive charts
- [Prism.js 1.29](https://cdnjs.cloudflare.com/ajax/libs/prism/) — Syntax highlighting
- [Google Fonts](https://fonts.googleapis.com/) — Inter & JetBrains Mono

After the initial load, the page functions fully offline.

> **Pyodide** (in-browser Python runtime) loads on demand when you click "Run in Browser" — first load takes 20–30 seconds and requires an internet connection.

## The Three-Equation Model

The core of the course is the canonical New Keynesian system:

$$x_t = E_t[x_{t+1}] - \frac{1}{\sigma}(i_t - E_t[\pi_{t+1}] - r_t^n)$$

$$\pi_t = \beta E_t[\pi_{t+1}] + \kappa x_t$$

$$i_t = \phi_\pi \pi_t + \phi_y x_t + v_t$$

The simulator solves this analytically using the method of undetermined coefficients: for an AR(1) shock with persistence ρ, the solution is $[a_x, a_\pi]^\top = (A - \rho B)^{-1} C$.

## Code Examples Included

| Topic | Python | R |
|---|---|---|
| Euler equation simulation | ✓ | ✓ |
| Calvo pricing & NKPC slope | ✓ | ✓ |
| Taylor rule dynamics & tradeoffs | ✓ | ✓ |
| NK model analytical solution | ✓ | ✓ |
| Blanchard-Kahn condition check | ✓ | ✓ |
| Kalman filter log-likelihood | ✓ | ✓ |
| Bayesian posterior mode estimation | ✓ | ✓ |
| Aiyagari (1994) steady state via VFI | ✓ | ✓ |

## Prerequisites

This course assumes familiarity with:
- Intermediate macroeconomics (IS-LM, Solow model)
- Calculus and linear algebra
- Basic probability and statistics

No prior DSGE knowledge required.

## References

- Galí, J. (2008). *Monetary Policy, Inflation, and the Business Cycle*. Princeton University Press.
- Woodford, M. (2003). *Interest and Prices*. Princeton University Press.
- Smets, F. & Wouters, R. (2007). Shocks and Frictions in US Business Cycles. *AER*, 97(3).
- Kydland, F. & Prescott, E. (1982). Time to Build and Aggregate Fluctuations. *Econometrica*, 50(6).
- Kaplan, G., Moll, B. & Violante, G. (2018). Monetary Policy According to HANK. *AER*, 108(3).
- Bernanke, B., Gertler, M. & Gilchrist, S. (1999). The Financial Accelerator in a Quantitative Business Cycle Framework. *Handbook of Macroeconomics*, Vol. 1C.
- Blanchard, O. & Kahn, C. (1980). The Solution of Linear Difference Models under Rational Expectations. *Econometrica*, 48(5).

## License

MIT License. Free to use, adapt, and distribute with attribution.
