# Accountability Graph Extraction

A computational framework for extracting accountability relationships 
from regulatory text and representing them as structured graphs.

## Research Question
Can accountability relationships in regulatory documents be 
represented as structured graphs, and do graph-level structural 
features predict convergence risk?

## Key Findings
- FDA Warning Letter corpus produces star-topology accountability 
  graphs with Firm as the dominant node (in-degree centrality = 0.444)
- Accountability openness score exhibits significant negative 
  correlation with PAC convergence risk 
  (Pearson r = −0.431, p = 0.0018; Spearman ρ = −0.742, p < 0.001)
- Cases cluster into three structural types: Open (n=16), 
  Standard (n=33), and Extreme convergence (n=1)
- WL2018-05 identified as extreme outlier across both 
  graph-based and PAC detection frameworks

## Methods
- Relation extraction (VIOLATES / INVOLVES / ATTRIBUTED_TO)
- Directed graph construction (networkx)
- Centrality analysis (in-degree, betweenness, PageRank)
- Composite accountability openness score
- K-means clustering + PCA
- Cross-project validation with PAC detection framework

## Dataset
FDA Warning Letter corpus (N=50, 21 CFR 210/211, 2016–2025)

## Related Projects
- [Premature Convergence Detection](https://github.com/sorakim-lab/premature-convergence-detection)

## Reference
Kim, S. (2026). Anticipated Accountability Convergence. SSRN 6371980.
