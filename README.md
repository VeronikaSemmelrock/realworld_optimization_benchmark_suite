
# Real-World Optimization Benchmark Suite
This repository is a curated collection of real-world optimization benchmark problems for ASP, CP, and general combinatorial optimization. 

All benchmark problems include at least:
- problem description 
- input instance files or generator files
- references to original sources

---

## Included Problem Families

### 1. House Configuration Problem (HCP)

The **House Configuration Problem (HCP)** is an abstraction of the real-world optimization task of configuring electronic systems. 
This repository includes the *adapted HCP*, which extends the original HCP with an ordering constraint for things and cabinets, used in the paper:

Semmelrock, V.; Friedrich, G. (2025).  
**Investigating the Grounding Bottleneck for a Large-Scale Configuration Problem: Existing Tools and Constraint-Aware Guessing**


#### Instance Generator

The generator `hcp/HCP_instanceGeneration.lp` produces valid HCP instances via 
`gringo HCP_instanceGeneration.lp  
--const numberOfPersons=5  
--const numberOfThingsPerPerson=10  
--text > instance_5p_10t.lp`

Change the constants to scale the instance.

#### Citations for HCP

If you use HCP data/encodings from this repository, please cite:

**Original HCP sources:**

- Friedrich, G.; Ryabokon, A.; Falkner, A. A.; Haselböck, A.; Schenner, G.; Schreiner, H. (2011).  
  **(Re)configuration using Answer Set Programming**  
  IJCAI Workshop on Configuration (ConfWS 2011).

- Ryabokon, A. (2015).  
  **Knowledge-Based (Re)Configuration of Complex Products and Services**  
  Dissertation, Alpen-Adria Universität Klagenfurt.

**Adapted HCP used here:**

- Semmelrock, V.; Friedrich, G. (2025).  
  **Investigating the Grounding Bottleneck for a Large-Scale Configuration Problem: Existing Tools and Constraint-Aware Guessing**

---

### 2. Partner Units Problem (PUP)

The **Partner Units Problem (PUP)** originates from configuration tasks in railway safety systems. 
The instances in this repository are a re-upload of the instances from the paper: 

Teppan, E., Friedrich, G., & Falkner, A. (2012). 
**QuickPup: A Heuristic Backtracking Algorithm for the Partner Units Configuration Problem** _Proceedings of the AAAI Conference on Artificial Intelligence_, _26_(2), 2329-2334. https://doi.org/10.1609/aaai.v26i2.18979 

#### Citations for PUP

If you use PUP instances, please cite:

- Teppan, E., Friedrich, G., & Falkner, A. (2012). **QuickPup: A Heuristic Backtracking Algorithm for the Partner Units Configuration Problem** _Proceedings of the AAAI Conference on Artificial Intelligence_, _26_(2), 2329-2334. https://doi.org/10.1609/aaai.v26i2.18979

---
## Contact
For questions, suggestions, or contributions, please contact veronika.semmelrock@aau.at 

## Citation for This Repository

If you use benchmarks from this repository, please cite the corresponding original problem. For citing the benchmark suite, please use:

```bibtex
@misc{realworldbenchmarks2025,
  author       = {Veronika Semmelrock},
  title        = {Real-World Optimization Benchmark Suite},
  year         = {2025},
  url          = {https://github.com/VeronikaSemmelrock/realworld_optimization_benchmark_suite},
  note         = {Online real-world optimization benchmark suite},
}
