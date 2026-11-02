# Public experimental data subset

This repository contains a selected public subset of data prepared for the N-1 supply-feasibility manuscript. It includes synthetic small-system inputs and results, IEEE 39-bus input and serialized records, and explicitly named IEEE 118-bus output tables. The 11-bus engineering case and records containing it are excluded from this public subset.

## Contents and provenance

- `dataset_inputs/`: MATPOWER case39 input and synthetic five-bus tables.
- `experiment_outputs/`: explicitly named IEEE 39 / IEEE 118 output tables and selected synthetic-case outputs, retained as source files without rerunning them.
- `research_evidence/`: IEEE 39 serialized records, MF-cycle arrays and mask manifest. The `attempt1_unknown` batch is a retained abandoned attempt, not part of the final batch.
- `research_evidence/4.2-mechanism-cases-public-subset.jsonl`: 12 non-11-bus records selected from a mixed 16-record source. The four 11-bus records were omitted; `4.2-subset-index.json` maps published zero-based indices to source indices.

The files are a partial data release, not a complete replication package: solver implementation and the excluded engineering-case data are not included. The results and source files have not been independently rerun or revalidated for this release. In particular, an unknown or timeout remains unresolved and must not be interpreted as infeasibility. Refer to the manuscript for model assumptions, coefficient encoding and scope.

The IEEE 39 input is derived from MATPOWER case39; retain the attribution and terms of the upstream distribution. `SHA256SUMS` provides file-level integrity, not scientific validation.
