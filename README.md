# Topology-Robust Power Flow Estimation using Graph
Neural Networks with Low-Rank Adapters

**Autores:** XXXXX XXXXX

## Abstract
Graph Neural Networks (GNNs) have emerged as effective data-driven
surrogates for AC power flow estimation, yet their performance often degrades
when the network topology changes due to switching, contingencies,
or reconfiguration. This work introduces PFGNNFlatAdapter, a topologyaware
learning framework that enhances generalization under structural variability
by applying low-rank residual updates over a fixed GNN backbone,
guided by a global mask that distinguishes nominal from perturbed operating
regimes. The model incorporates physically grounded covariates, including
active and reactive power injections (P, Q) and a one-hot encoding of the
bus type (Slack, PV, PQ), together with a structural covariate Z that captures
local topological changes at the node level. In addition, including an
N−k augmentation strategy, extended up to N−3, preserves graph connectivity
and avoids isolated nodes, generating diverse yet physically meaningful
training conditions. A dynamic edge index is included for each sample, allowing
the model to operate directly on varying graph structures without
retraining. Experiments on the 14, 30, and 118 bus pandapower systems
show that the proposed approach maintains high accuracy in nominal conditions
(MAPE below 0.1%) while achieving strong robustness under topological
perturbations (global MAPE below 1% across all cases), with near-linear
growth in parameters and runtime. These results indicate that adapter-based
GNN architectures offer a promising and computationally efficient direction
for topology-aware power flow estimation in modern, dynamically evolving
power grids.

## Estructura del repositorio
- /code : scripts de entrenamiento e inferencia
- /data : datasets y archivos grandes
- /figures : figuras PNG/PDF/SVG
- /docs : borradores y LaTeX

## Cómo reproducir
1. pip install -r requirements.txt
2. Ejecutar notebooks y scripts en /code

## Licencia
MIT
