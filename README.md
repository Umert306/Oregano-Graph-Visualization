# OREGANO Knowledge Graph and Ontology Construction

This notebook builds a biomedical knowledge graph and an OWL ontology from the **OREGANO V2.1 dataset**.  
It extracts entities and relationships from subject–predicate–object triples, constructs an ontology using **Owlready2**, generates strict **First-Order Logic (FOL)** statements, and produces an interactive visualization of the graph.

---

## Features

### 1. Ontology Construction
- Creates **OWL classes** for all unique subject and object nodes.  
- Creates **OWL object properties** for each predicate.  
- Assigns **domain** and **range** constraints for all relationships.  
- Saves the ontology as an **.owl file**.

---

### 2. Quantifier Analysis and FOL Generation
- Computes frequency patterns between subjects and objects.  
- Classifies relations as **universal**, **many**, or **existential**.  
- Generates strict **First-Order Logic statements** for every relation type.

---

### 3. Knowledge Graph Visualization
- Builds an interactive **PyVis** knowledge graph.  
- Colors nodes based on entity type.  
- Saves the visualization as an **HTML** file.

---

### 4. Dataset Insights
- Counts **unique subjects**, **objects**, and **relations**.  
- Computes **total triples**, **node types**, and **relation distributions**.

---
