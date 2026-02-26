# 📘 Project 5 Documentation: Access KEGG Pathway Database

## 🧬 Overview

This project demonstrates how to **programmatically interface with the KEGG (Kyoto Encyclopedia of Genes and Genomes) database** using **Biopython’s REST API**. It focuses on automating the retrieval of the **TP53 gene entry**, performing custom parsing to identify signaling pathways, and visualizing biological interaction maps.

---

## 🛠 Requirements

- Python 3.x  
- Biopython  
- Internet access for KEGG API requests  
- Python notebook environment (Kaggle, Jupyter, or Google Colab)

---

## 🧬 Access KEGG Pathway Data

### 🎯 Objective

To **retrieve**, **parse**, and **visualize** the signaling pathways associated with the **Human TP53 gene (ID: 7157)**, including:

- Fetching raw gene data via REST API  
- Dynamically searching and extracting specific Pathway IDs (hsa04115)  
- Rendering high-resolution biological pathway maps directly in the workspace

### 📁 Dataset

- [KEGG Gene: hsa:7157 (TP53)](https://www.genome.jp/dbget-bin/www_bget?hsa:7157)
- [KEGG Pathway: hsa04115 (p53 signaling pathway)](https://www.genome.jp/kegg-bin/show_pathway?hsa04115)

### 📓 Notebook

- [View Python Notebook](https://github.com/sheetalreddy25/Bio-Python-Labs/blob/e9686318d4ab065ea55adb5facf97635ebafc3bf/access-kegg-database.ipynb)

### 🔄 Workflow

1. Import **Biopython KEGG REST** and **Gene Parser** modules.
2. Fetch the raw record for **hsa:7157** and save it as a local text file for persistence.
3. Parse the local file to extract basic metadata (Gene ID and Name).
4. Implement a **custom search algorithm** to scan the raw data for the specific "p53 signaling pathway" ID.
5. Extract the discovered ID (**hsa04115**) while cleaning technical tags from the pathway name.
6. Use the extracted ID to request the **pathway diagram (image)** from the KEGG server.
7. Display the biological map using `IPython.display`.

---

## 📊 Key Takeaways

- **Automation:** The script dynamically "finds" the pathway ID rather than using hardcoded values.
- **Data Persistence:** Saving API results locally allows for efficient offline parsing and debugging.
- **Visualization:** Integrating KEGG images provides immediate biological context to genomic data analysis.

---

## 📚 References

- [KEGG: Kyoto Encyclopedia of Genes and Genomes](https://www.genome.jp/kegg/)
- [Biopython KEGG Module Documentation](https://biopython.org/docs/1.75/api/Bio.KEGG.REST.html)
- [KEGG Gene Entry: 7157](https://www.genome.jp/dbget-bin/www_bget?hsa:7157)
