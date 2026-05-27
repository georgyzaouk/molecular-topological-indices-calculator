# Topological Indices Calculator

A Python/Jupyter Notebook project for computing molecular topological indices from chemical structure files.

This project calculates three graph-based molecular descriptors:

- Edge Density
- Wiener Index
- Petitjean Index

The project was completed as part of a coding assignment for the Computational Biology course at the Lebanese American University.

## Overview

Molecules can be represented as graphs, where atoms are treated as nodes and bonds are treated as edges. This project uses that graph representation to calculate topological indices that describe molecular structure and connectivity.

The notebook supports molecular input files and computes the selected index or all available indices for each molecule.

## Background

Topological indices are numerical descriptors that represent the connectivity of a molecular structure. In this project, molecules are modeled as graphs, where atoms are represented as nodes and bonds as edges.

These indices are useful in chemoinformatics and molecular modeling because they provide a fast, graph-based way to describe molecular structure. They can support applications such as molecular comparison, similarity search, QSAR modeling, and drug discovery.

## Features

- Computes Edge Density
- Computes Wiener Index
- Computes Petitjean Index
- Supports `.mol` files
- Supports `.sdf` files containing multiple molecular structures
- Supports folders containing multiple `.mol` files
- Displays molecule names with computed index values
- Implements calculations from graph operations rather than using built-in topological index functions

## Technologies Used

- Python
- Jupyter Notebook
- NetworkX
- RDKit
- Matplotlib

## Repository Structure

```text
topological-indices-calculator/
├── README.md
├── notebook/
│   └── topological_indices_calculator.ipynb
└── test_cases/
    ├── mol/
    ├── sdf/
    └── archives/
```

## Folder Description

- `notebook/`: Contains the main Jupyter Notebook used to compute the topological indices.
- `test_cases/mol/`: Contains individual `.mol` test files.
- `test_cases/sdf/`: Contains `.sdf` files, including files with multiple molecular structures.
- `test_cases/archives/`: Contains compressed test case archives used during validation.

## Indices Computed

### Edge Density

Edge Density measures how connected a molecular graph is by comparing the number of existing bonds to the maximum possible number of bonds between atoms.

### Wiener Index

The Wiener Index is calculated as the sum of the shortest path distances between all pairs of atoms in the molecular graph.

### Petitjean Index

The Petitjean Index is based on the graph diameter and radius, providing a measure of molecular shape and graph compactness.

## Usage

Open the notebook:

```text
notebook/topological_indices_calculator.ipynb
```

Then run the cells and provide one of the supported input types:

- a single `.mol` file
- a folder containing multiple `.mol` files
- an `.sdf` file containing multiple molecular structures

The notebook will output the molecule names along with the selected computed indices.

## Example Output

```text
Molecule: Structure2D_COMPOUND_CID_21013
Edge Density: ...
Wiener Index: ...
Petitjean Index: ...
```

## Notes

The calculations are implemented manually using graph operations. Built-in functions that directly compute Edge Density, Wiener Index, or Petitjean Index are not used.

## Authors

- Georgy Zaouk
- Kassem Rammal

## Course

Computational Biology  
Lebanese American University
