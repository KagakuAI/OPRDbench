OPRDbench: A Manufacturing Chemistry Benchmark for CASP Tools
--------------------------------------------------------------------------------

This repository contains a benchmark dataset of target molecules extracted from the 
Organic Process Research & Development (OPRD) journal,
intended for the evaluation of Computer-Aided Synthesis Planning (CASP) tools on
manufacturing-relevant chemistry.

Motivation
--------------------------------------------------------------------------------

Current Computer-Aided Synthesis Planning (CASP) tools and benchmarks are biased toward medicinal chemistry.
Manufacturing routes, as reported in OPRD, are optimized for industrial-scale production
and differ substantially from discovery routes in terms of reaction choice, reagent
availability, cost, and process safety. This benchmark provides a resource for
evaluating and improving CASP tools in this domain.

Dataset
--------------------------------------------------------------------------------

The dataset ``OPRDtargets.csv`` currently contains **211 target molecules** drawn from OPRD publications,
representing approximately **5% of the papers processed** so far. The collection is being actively expanded.

Each entry consists of:

- **TITLE** - the title of the original OPRD publication reporting the manufacturing route
- **DOI** - the DOI of the original OPRD publication reporting the manufacturing route
- **SMILES** - the target molecule in SMILES format

The dataset contains only target structures and literature references.
Synthetic routes are **not** included and can be retrieved from the cited publications.

Usage
--------------------------------------------------------------------------------

The targets can be directly loaded into CASP tools for benchmarking. 
Each predicted route can then be compared with the manufacturing route reported in the original publication via the provided DOI.