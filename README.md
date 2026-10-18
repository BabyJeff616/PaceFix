# PaceFix

PaceFix is a multi-candidate iterative framework for LLM-based automated program repair (APR). It uses information from candidate patches to guide subsequent repair rounds.

## Approach

PaceFix combines two complementary components:

- **State Decision** selects the program to continue repairing from candidates with the maximum functional progress, using failure-related evidence and deterministic fallback rules.
- **Structural Aggregation** summarizes shared AST edit patterns across a progress-conditioned candidate cohort and converts them into feedback for the next repair round.

The selected program and structural feedback jointly guide next-round patch generation.

## Repository Contents

The repository provides the PaceFix source code, experiment scripts, and benchmark input files for Defects4J experiments. The implementation uses Joern for program analysis and GumTree for AST differencing.

Download and extract `PaceFix.zip` to access the files. Configure the model API settings, dependencies, and local tool paths before running the experiments.
