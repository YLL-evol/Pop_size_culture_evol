# Pop_size_culture_evol
Simulation of population structure, migration, innovation, and social learning strategies interact to shape the evolution of cultural complexity.

# Cultural Evolution Simulation Framework  
## Population Size, Migration, and Cumulative Culture Dynamics

---

# 1. Overview of the Framework

This repository presents a **computational model of cumulative cultural evolution**, inspired by experimental and theoretical work in cultural evolution, particularly the research tradition of:

- Derex (2013)
- Derex (2018)
- Henrich (2004), Boyd & Richerson (1985), Mesoudi (2011)

The framework simulates how **population structure, migration, innovation, and social learning strategies** interact to shape the evolution of cultural complexity.

---

## What this framework does

This model allows you to:

- Simulate **cumulative cultural evolution over generations**
- Test effects of:
  - population size
  - migration between groups
  - innovation rate
  - social learning bias (payoff + conformist learning)
- Track:
  - cultural performance (multi-trait or scalar)
  - innovation dynamics
  - cultural diversity
  - between-group divergence

---

## Biological / Anthropological questions it addresses

This framework can be used to study:

- Why do larger populations maintain more complex culture?
- How does migration affect cultural convergence or divergence?
- When does innovation matter vs selection?
- What mechanisms drive cumulative cultural evolution?
- How does structure of populations shape cultural adaptation?

---

## Data source

This project uses:

### Simulated agent-based data
Generated within the notebook:
- Individual-level cultural traits
- Group membership
- Generation time steps
- Innovation events

---

## Key references (conceptual foundation)

- Derex et al. 2013, PNAS — cumulative culture in transmission chains  
- Derex et al. 2018, Nature Communications — population size and culture  
- Henrich 2004, American Antiquity — demographic cultural evolution  
- Boyd & Richerson 1985 — cultural transmission theory  
- Mesoudi 2011 — cultural evolution framework

---

# 2. Model Design Schema

## 2.1 Conceptual model structure

```
                Population Structure
           (size, groups, migration rate)
                         │
                         ▼
            Individual Cultural State
        (multi-trait or scalar performance)
                         │
     ┌───────────────────┼───────────────────┐
     ▼                   ▼                   ▼
Innovation       Social Learning       Migration
(random noise)   (biased copying)     (between groups)
     └───────────────────┼───────────────────┘
                         ▼
               Cultural Fitness
        (selection of high-performance traits)
                         ▼
               Next Generation State
```

---

## 2.2 Computational workflow schema

| Step | Process | Input | Output |
|------|--------|-------|--------|
| 1 | Environment setup | None | Python environment |
| 2 | Parameter definition | user settings | simulation config |
| 3 | Simulation engine | parameters | raw agent dataset (.csv-like table) |
| 4 | Data inspection | raw dataset | structure summary |
| 5 | Descriptive statistics | dataset | statistical tables |
| 6 | Quality control | dataset | cleaned dataset |
| 7 | Cumulative culture analysis | cleaned dataset | plots + regression |
| 8 | Population size effect | cleaned dataset | statistical comparison |
| 9 | Migration analysis | cleaned dataset | convergence plots |
| 10 | Innovation dynamics | cleaned dataset | time series plots |
| 11 | Diversity analysis | cleaned dataset | variance metrics |
| 12 | Final synthesis | all outputs | summary figures |

---

# 3. Explanation of Each Analysis Step

---

## Step 1 — Environment setup

Ensures reproducibility using standard scientific Python stack:
- numpy
- pandas
- matplotlib
- seaborn
- scipy

Purpose:
Guarantees reproducibility and comparability across runs.

---

## Step 2 — Parameter definition

Defines:

- population sizes
- migration rate
- innovation rate
- learning bias parameters

Mechanism:
These parameters represent **cultural transmission ecology**.

Reference:
Boyd & Richerson (1985) — cultural transmission theory

---

## Step 3 — Simulation engine

Agent-based model generating:

- individual cultural traits
- learning decisions
- innovation events
- migration events

Mechanism:
Each agent updates cultural state via:
- innovation (random generation)
- social learning (biased copying)
- migration (cross-group transmission)

Reference:
Derex et al. 2013 — transmission chain experiments

Why this method:
Captures **micro-level mechanisms generating macro cultural patterns**

---

## Step 4 — Data inspection

Checks:

- data types
- structure
- missing values
- ranges

Purpose:
Ensures simulation validity and avoids structural bias.

---

## Step 5 — Descriptive statistics

Outputs:

- mean cultural performance
- variance
- distribution shapes

Why:
Establishes baseline structure of cultural system.

---

## Step 6 — Data quality control

Includes:

- missing values check
- outlier detection
- distribution diagnostics

Why:
Ensures observed patterns are not artifacts of simulation noise.

---

## Step 7 — Cumulative culture analysis

Method:
Time-series regression of cultural performance over generations.

Mechanism:
Tests whether culture accumulates through iterative improvement.

Reference:
Henrich (2004)

Why this method:
Captures **core signature of cumulative cultural evolution**

---

## Step 8 — Population size effect

Method:
Comparison of cultural performance across group sizes.

Mechanism:
Larger groups increase:
- probability of innovation
- retention of high-quality traits

Reference:
Derex et al. 2018 Nature Communications

---

## Step 9 — Migration analysis

Method:
Tracking convergence of cultural traits across groups.

Mechanism:
Migration increases cultural homogenization.

Why this method:
Direct test of **population connectivity hypothesis**

---

## Step 10 — Innovation dynamics

Method:
Tracking innovation frequency over time.

Mechanism:
Innovation typically high early, then declines due to selection.

Reference:
Boyd & Richerson (1985)

---

## Step 11 — Cultural diversity analysis

Method:
Variance of cultural traits across time.

Mechanism:
Measures:
- divergence
- convergence
- cultural drift

---

## Step 12 — Final synthesis

Combines all metrics:

- cumulative growth
- diversity collapse
- selection dominance
- group effects

Purpose:
Integrates mechanisms into single evolutionary narrative.

---

# 4. How to read results

## Key interpretation guide

### If cultural performance increases:
→ evidence of cumulative cultural evolution

### If population size increases performance:
→ demographic cultural effect

### If variance decreases:
→ cultural convergence or strong selection

### If innovation decreases over time:
→ selection dominates exploration

### If groups converge:
→ strong migration or cultural diffusion

---

## What counts as a strong result?

A publishable pattern typically includes:

- upward cultural trajectory
- statistically significant population effect
- structured variance reduction
- mechanistic consistency across analyses

---

# 5. Conclusion

This framework demonstrates how:

- micro-level learning rules
- population structure
- migration processes

jointly generate **macroscopic cultural evolution patterns**.

It provides a mechanistic bridge between:

- experimental cultural evolution (Derex-style transmission chains)
- theoretical models (Henrich, Boyd & Richerson)
- simulation-based evolutionary dynamics

The model is intentionally simple but extensible, allowing integration with empirical datasets or more complex cognitive rules.

---

# 6. References 

Boyd, Robert, and Peter J. Richerson. 1985. *Culture and the Evolutionary Process*. Chicago: University of Chicago Press.  
https://www.press.uchicago.edu/ucp/books/book/chicago/C/bo3630708.html  

Derex, Maxime, et al. 2013. “Experimental Evidence for the Influence of Group Size on Cultural Complexity.” *Proceedings of the National Academy of Sciences* 110 (41): 16730–16735.  
https://www.pnas.org/doi/10.1073/pnas.1305527110  

Derex, Maxime, et al. 2018. “Population Structure and Cultural Evolution.” *Nature Communications* 9: 2112.  
https://www.nature.com/articles/s41467-018-06508-9  

Henrich, Joseph. “Demography and Cultural Evolution: How Adaptive Cultural Processes Can Produce Maladaptive Losses—The Tasmanian Case.” American Antiquity 69, no. 2 (2004): 197–214. https://doi.org/10.2307/4128416.

Mesoudi, Alex. 2011. *Cultural Evolution: How Darwinian Theory Can Explain Human Culture and Synthesize the Social Sciences*. Chicago: University of Chicago Press.  
https://press.uchicago.edu/ucp/books/book/chicago/C/bo10360088.html  

Rendell, Luke, et al. 2010. “Why Copy Others? Insights from the Social Learning Strategies Tournament.” *Science* 328 (5975): 208–213.  
https://www.science.org/doi/10.1126/science.1184719  

---

```
