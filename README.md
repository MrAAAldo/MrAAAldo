## Aldo Mendoza

Actuary working on one question in five markets: **what is the optimal decision under
uncertainty, and how do I honestly measure whether I have an edge?**

Auctions and pricing · stochastic control (HJB) · causal inference under censoring.

---

**What I work on**

- **Pricing under censored outcomes.** In a first-price auction you learn the clearing
  price only when you win; lose, and all you know is `price > your_bid`. That same
  structure is a claim above a policy limit, an unfilled limit order, a quoted strike.
  Most systems patch it by assuming a parametric form. I measure what that assumption
  costs — in my own bid-landscape work, handling the censoring correctly contributed
  roughly **5× more than model sophistication did**.
- **Stochastic control.** My thesis derives and solves the Hamilton-Jacobi-Bellman
  equation for the Merton problem under Vasicek rates, with closed-form HARA policies
  proved via a verification theorem — and reports honestly that the optimal policy did
  **not** beat the 1/N benchmark out-of-sample (Sharpe 0.88 vs 0.99).
- **Production systems.** A seven-engine pricing system (shadow mode) reconciled to the
  cent against $24.3M of direct revenue, where 83% of outcomes are never observed.

**How I work**

I kill my own results before anyone else has to. I separate revenue *captured* from
revenue *identified*. When a signal-value estimate turned out to overstate its effect
threefold under Simpson's bias, I shipped the correction rather than the flattering
number — and when an earlier bid-landscape model showed a large gain, I found it had
been measured against a strawman baseline and published the smaller, real one instead.

---

| Repo | What it is |
|---|---|
| [**stochastic-portfolio-platform**](https://github.com/MrAAAldo/stochastic-portfolio-platform) | Operational artifact of the thesis (FCFM-BUAP, 2026). HJB / verification theorem / HARA Stone-Geary solver as a runnable CLI platform: walk-forward backtesting, risk gates, paper trading. Analytical solver cross-checked against a DQN agent and 1,000-path Monte Carlo. 590 tests. |

Work on bid-landscape estimation, sports-market pricing and multi-agent production
systems lives in private repositories — happy to walk through any of it in a screen share.

---

📍 Mexico City · EN/ES
📄 Thesis: *Stochastic Control in Investment Portfolio Optimization* — 262 pp.
💼 [LinkedIn](https://www.linkedin.com/in/aldo-mendoza-63aa03234)
