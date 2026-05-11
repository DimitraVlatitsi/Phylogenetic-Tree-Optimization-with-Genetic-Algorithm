# Weighted Phylogenetic Tree Optimization using Genetic Algorithm

This project implements a stochastic optimization approach for improving phylogenetic tree reconstruction using a Genetic Algorithm (GA). The algorithm learns optimal weights for different mutation types in a weighted distance matrix to improve tree accuracy.

---

## 🔬 Method Overview

- Sequence alignment is parsed using **Biopython**
- Sites are classified into:
  - SNP positions
  - INDEL positions
  - Microsatellite regions
- A weighted pairwise distance matrix is constructed
- Neighbor-Joining (NJ) trees are generated
- Tree quality is evaluated using **Robinson–Foulds (RF) distance** against a reference tree
- A Genetic Algorithm optimizes mutation weights to minimize RF distance

---

## ⚙️ Optimization

The Genetic Algorithm evolves weights for:

- SNP contribution  
- INDEL penalty  
- Microsatellite weight  

**Fitness function:** Minimization of RF distance

---

## 📦 Requirements

Install dependencies:

```bash
pip install -r requirements.txt
