# Protein Sequence-Structure Database and Machine Learning Analysis

This repository presents a protein informatics workflow that combines database engineering, protein structure analysis, and machine learning. The project is organized around two connected goals: building structured protein sequence and structure databases from primary biological data sources, and using those curated datasets for statistical and predictive analysis of secondary and tertiary structure patterns.

The code highlights experience in:

- Creating protein sequence and structure databases from heterogeneous source files
- Parsing and standardizing data from PDB, PDBsum, and PISCES
- Mapping protein chains to corresponding nucleotide sequences with TBLASTN-based matching and sequence cleaning
- Performing 3D Delaunay tessellation on protein structures to characterize residue neighborhoods
- Designing SQLite databases for downstream structural and protein-protein interaction analysis
- Running statistical analysis on tessellation-derived features, including simplex log-likelihood calculations and hypothesis testing
- Applying machine learning and deep learning methods to secondary structure classification, clustering, and assignment
- Investigating codon-level protein-protein interfaces and the relationship between mutagenesis and structure-derived likelihood potentials

## Project Structure

### 1. Protein Sequence and Structure Database Creation

This part of the project focuses on constructing analysis-ready protein datasets from raw structural and sequence resources.

Key workflow components:

- Parse original files from PDB, PDBsum, and PISCES
- Extract corresponding DNA sequences with TBLASTN
- Clean and reconcile protein and nucleotide sequence matches
- Reformat matched results into PDB-compatible chain-level files
- Integrate residue coordinates, codons, and DSSP secondary structure annotations
- Perform 3D tessellation of protein structures
- Build SQL databases for individual-chain and protein-protein interaction analysis


### 2. Protein Sequence, Secondary Structure, and Tertiary Structure Analysis

This part of the project uses the curated databases and tessellation outputs to study structural organization and build predictive models.

Key analysis themes:

- Statistical analysis of tessellated structures
- Calculation of log-likelihood ratios for simplices
- Hypothesis testing on structure-derived variables
- Secondary structure classification, clustering, and assignment
- Machine learning analysis of twisted beta-strands
- Deep learning-based secondary structure assignment
- Codon-level analysis of protein-protein interfaces
- Exploration of relationships between mutagenesis and log-likelihood potentials at the structural level

