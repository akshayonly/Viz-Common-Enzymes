# Comparative Enzyme-Disease Network Analysis from PubMed Literature
### A Graph-Based Approach to Biomedical Insight

This project builds and visualizes enzyme-centric knowledge graphs by mining biomedical literature from PubMed. It focuses on comparing how different enzymes—defined by their Enzyme Commission (EC) numbers—are associated with specific diseases such as **Cancer** and **SARS-CoV-2**.

By mapping co-mentions of enzymes across thousands of research articles, this pipeline enables a data-driven exploration of enzyme-disease associations within the scientific literature.

---

## 🚀 Project Overview

![Pipeline Diagram](https://raw.githubusercontent.com/akshayonly/Enzymes-Network-Graph/main/Common-Enzymes-Detail.drawio.png)

This pipeline includes the following steps:

1. **PMID Extraction**  
   Collect disease-specific publication IDs from PubMed using automated search or manual input.

2. **Metadata Retrieval**  
   Fetch complete MEDLINE records for each publication using the NCBI Entrez API.

3. **Enzyme Detection**  
   Extract EC-numbered enzyme mentions from the `RN` (Registry Number) field.

4. **Graph Construction**  
   Build a bipartite network where:
   - Nodes represent **PMIDs** and **enzymes**
   - Edges represent co-mentions in a publication

5. **Interactive Visualization**  
   Render the graph using **PyVis** for interactive exploration, with enzyme classes visually grouped.

6. **Graph Export**  
   Export the network in both **HTML** (browser-based view) and **GraphML** (for Cytoscape/Gephi) formats.

---

## 🧪 Use Cases

- Identify and compare enzyme involvement across different diseases
- Discover potential **biomarkers** or **shared therapeutic targets**
- Track research trends or gaps in enzyme-related disease studies
- Generate hypotheses from high-level literature association maps

---

## 📈 Example Output

Visualizations are enriched by enzyme class and publication links.

![HTML Visualization 1](https://raw.githubusercontent.com/akshayonly/Enzymes-Network-Graph/main/Screenshot%202022-03-11%20165751.png)

![HTML Visualization 2](https://raw.githubusercontent.com/akshayonly/Enzymes-Network-Graph/main/Screenshot%202022-03-11%20165902.png)

- Enzyme nodes are colored by diseases (e.g., Covid-19 and Cancer).
- Interactive output allows zoom, search, and node inspection.

---

## 🧠 What's Next?

This foundation can be extended with:

- **Edge weighting** based on enzyme frequency or co-occurrence strength
- **Semantic enrichment** from MeSH terms or abstracts
- **Temporal tracking** of enzyme-disease focus over time
- **Disease-disease comparison** graphs based on enzyme overlap

---

Feel free to fork the repository or raise issues for improvements. For citation or integration into a pipeline, please contact the author.
