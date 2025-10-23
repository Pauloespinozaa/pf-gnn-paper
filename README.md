# Robust Power Flow Estimation under Topological Variations via Graph Neural Networks with Flat Adapters

**Autores:** XXXXXz

## Abstract
Graph Neural Networks (GNNs) have recently emerged as powerful data-driven surrogates for AC power flow estimation, yet their performance often deteriorates under structural variability caused by switching operations or contingency events. This paper presents PFGNNFlatAdapter, a topology-aware architecture that combines topological data augmentation with a low-rank residual adapter to improve robustness without compromising nominal accuracy. The model integrates electrical features (P,Q,Z), bus-type encodings, and a binary connectivity indicator to explicitly capture the local impact of network reconfigurations on global voltage and phase-angle dynamics. Experimental results on the IEEE 14-, 30-, and 118-bus test systems demonstrate state-of-the-art accuracy across both nominal and perturbed topologies, achieving MAPE below 0.2% and R2 > 0.999 in all cases. The framework scales linearly in training time (from 1.3x10^3 s to 2.2x10^3 s) while maintaining stable convergence and consistent error distribution. These findings confirm that combining physically grounded features with parameter-efficient adapters enables robust, scalable, and topology-generalizable power flow estimation for dynamic electrical grids. Compared to a baseline, the proposed model achieves over two orders of magnitude reduction in error under perturbed topologies (MAPE 0.19% vs. 28.6%) while preserving near-perfect accuracy in nominal conditions, confirming its superior robustness and generalization capability.

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
