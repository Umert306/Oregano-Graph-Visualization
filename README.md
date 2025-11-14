# Oregano-Graph-Visualization

OREGANO Knowledge Graph and Ontology Construction

This project builds a biomedical knowledge graph and an OWL ontology from the OREGANO V2.1 dataset. It extracts entities, relationships, and structure from subject–predicate–object triples, visualizes the graph, and generates a machine-readable ontology using Owlready2. The result is a structured semantic representation of compounds, genes, proteins, diseases, and other biological concepts that can be used for reasoning, querying, and downstream knowledge engineering tasks.

Overview

The repository contains:

Data loading and preprocessing for the OREGANO TSV dataset.

Automated construction of OWL classes and object properties based on the dataset.

Domain and range assignment for each relationship using frequency-driven quantifier rules.

Generation of strict first-order logic statements describing relationship semantics.

Interactive knowledge graph visualizations using PyVis.

Export of a complete OWL ontology file for reuse.

Features
1. Ontology Generation

The ontology is created programmatically using Owlready2.

Each unique node type in the dataset becomes an OWL class that inherits from Thing.

Each predicate is converted into an OWL object property.

Domain and range assignments are inferred from subject and object distributions.

Output is saved as an .owl file compatible with Protégé.

2. Relationship Quantification

The project examines the frequency of each subject-object pair within a given predicate. Based on the proportion of occurrences, relationships are classified as:

Universal (for all)

Many

Existential

These classifications are then converted into formal first-order logic expressions in strict notation.

3. Knowledge Graph Visualization

A subgraph is sampled and visualized using PyVis.

Nodes are colored by category

Edge types are labeled with predicate names

The final visualization is rendered as an HTML file for interactive exploration

4. High-Level Statistics

The project reports dataset-level metrics, including:

Number of unique subjects

Number of object types

Number of predicates

Total number of edges

Relationship distributions
