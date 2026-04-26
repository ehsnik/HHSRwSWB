# HHSRwSWB
Home Healthcare Scheduling and Routing with Synchronization and Workload Balance

# Home Healthcare Scheduling and Routing – Benchmark Instances

This repository contains the benchmark instances developed for the paper:

> Amini-Rarani, M., Nikbakhsh, E., Mahnam, M., & Zegordi, S.H. (2026).  
> *A column generation-based heuristic algorithm for home healthcare scheduling and routing with synchronization and workload balance.*  
> Faculty of Industrial and Systems Engineering, Tarbiat Modares University, Tehran, Iran.

---

## 1. Problem Description

Home healthcare includes medical and support services provided at patients’ homes to help them manage medical conditions, maintain comfort, and reduce in-person visits to healthcare centers.

This study develops a mathematical model for the **Home Healthcare Scheduling and Routing Problem (HHC-SRP)** over a daily planning horizon. The model integrates:

- Caregiver scheduling and routing decisions
- Synchronization for patients requiring **two caregivers**
- Minimization of arrival time differences for synchronized visits
- High-priority patient handling
- Workload balancing among caregivers
- Reduction of total working time
- Patient satisfaction factors:
  - Preferred time windows
  - Gender preferences
  - Caregiver–patient loyalty
- Caregiver fatigue modeling
- Time-dependent travel times

To solve the problem efficiently, a **column generation-based heuristic algorithm** is proposed. The pricing subproblem (i.e., caregiver routing) is solved using a customized labeling algorithm incorporating several feasibility and dominance features.

Computational experiments show:
- Up to **99% reduction in computational time**
- Near-optimal solution gaps:
  - 0.53% for small instances
  - -2% for large instances
- A real-world case study demonstrates a **22.9% improvement** over the current operational plan.

---

## 2. Repository Contents
├── instances/

│ ├── small/

│ ├── medium/

│ ├── large/

└── README.md


### 3. Folder Description

- `instances/small/`  
  Small-scale synthetic instances used for validation and comparison.

- `instances/medium/`  
  Medium-scale benchmark instances.

- `instances/large/`  
  Large-scale instances used to evaluate computational performance.
  
---

## 4. Instance Descriptions

Please see the Data_Description.pdf file in the root of the Instances folder.

## 5. Usage

These instances can be used to:

- Benchmark exact algorithms
- Test heuristic or metaheuristic methods
- Compare column generation implementations
- Study synchronization-constrained routing
- Analyze workload balancing mechanisms
  
---

## 6. Computational Performance Summary

Across generated instances:

- Computational time reduced by up to **99%**
- Average optimality gap:
  - 0.53% (small instances)
  - -2% (large instances)
- Real case study (instance not provided here due to confidentiality restrictions):
  - 22.9% improvement over current operational plan

---

## 7. Contact
For questions regarding the instances or implementation details, please contact the authors via their institutional affiliation. Right now, the corresponding author is Ehsan Nikbakhsh (reachable via nikbakhsh@modares.ac.ir)

---

## 8. Citation

If you use these instances in your research, please cite:

Amini-Rarani, M., Nikbakhsh, E., Mahnam, M., & Zegordi, S.H. (2026).  
*A column generation-based heuristic algorithm for home healthcare scheduling and routing with synchronization and workload balance.*  
Faculty of Industrial and Systems Engineering, Tarbiat Modares University, Tehran, Iran.

Example BibTeX:
```bibtex
@article{AminiRarani2026HHC,
  author  = {Amini-Rarani, M. and Nikbakhsh, E. and Mahnam, M. and Zegordi, S. H.},
  title   = {A column generation-based heuristic algorithm for home healthcare scheduling and routing with synchronization and workload balance},
  year    = {2026},
  institution = {Faculty of Industrial and Systems Engineering, Tarbiat Modares University, Tehran, Iran}
}
