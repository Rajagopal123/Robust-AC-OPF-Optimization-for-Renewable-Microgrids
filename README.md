
## **Robust AC-OPF Optimization for Renewable Microgrids**

This project presents a **robust multi-objective AC Optimal Power Flow (AC-OPF)** framework for a renewable-dominated microgrid, incorporating uncertainty in load and renewable generation.

The model is implemented on a modified **IEEE 30-bus system** and uses **NSGA-II** to obtain Pareto-optimal solutions balancing economic, environmental, and operational objectives.

---

## **Problem Statement**

Traditional OPF methods assume deterministic conditions and fail under renewable variability.
This project addresses this by developing a **robust OPF framework** that ensures feasible and reliable operation under uncertainty.

---

## **Key Features**

* Multi-objective optimization: **cost, emission, voltage deviation, renewable utilization**
* **Scenario-based uncertainty modeling** (PV, wind, load, price)
* **Monte Carlo scenario generation (100 scenarios)**
* **K-means clustering for scenario reduction (~15 scenarios)**
* **NSGA-II based Pareto optimization**
* Comparison of **Deterministic, Stochastic, and Robust OPF**

---

## **System Details**

* Test System: **IEEE 30-bus microgrid**
* Base Power: **100 MVA**
* Components:

  * Grid (Slack Bus – 300 MW)
  * Diesel Generator (25 MW)
  * Battery Storage (20 MW)
  * Solar PV (45 MW)
  * Wind Farm (35 MW)

---

## **Methodology**

1. Load system data using MATPOWER
2. Generate uncertainty scenarios using Monte Carlo simulation
3. Reduce scenarios using K-means clustering
4. Evaluate each solution across all scenarios
5. Apply NSGA-II for multi-objective optimization
6. Extract Pareto-optimal solutions
7. Select best compromise solution (knee point)

---

## **Key Results**

* Scenario reduction: **100 → ~15 scenarios**
* Robust OPF ensures **feasible operation under uncertainty**
* Trade-offs observed between:

  * Cost vs Emission
  * Cost vs Voltage Stability
* Robust solution prioritizes **system reliability over cost**
* Example result:

  * Cost ≈ **611,993 Rs/hour**
  * Emission ≈ **59.56 ton/hour**

---

## **Tools Used**

* MATLAB
* MATPOWER
* NSGA-II Algorithm
* K-means Clustering

---

## **Repository Structure** *(edit based on your files)*

```
/code          → MATLAB scripts
/data          → MATPOWER case files
/results       → plots and outputs
/report        → project report / PPT
```

---

## **Future Work**

* Time-series (multi-hour) OPF
* AI-based forecasting integration
* Real-time implementation
* Larger power system validation

---

## **Author**

Rajagopal B
B.Tech Electrical and Electronics Engineering



If you want:
👉 I can also **review your GitHub repo structure before you upload** (this matters more than you think).
