# 🧬 My Bio Hub – A Collection of Bioinformatics Projects

Welcome to **My Bio Hub**, a personal repository showcasing projects I've built while learning and applying core techniques in bioinformatics.

## 🔬 What's Inside?

### 📘 Accessing Bioinformatics Databases using Biopython
- Sequence alignment using NCBI BLAST (BLASTn & BLASTp)  
- Literature retrieval and nucleotide access via Entrez API (PubMed, Nucleotide)  
- Protein structure & domain analysis (PDB, PROSITE, SCANPROSITE)  
- Pathway and gene network exploration (KEGG)  

---

## 🚀 Completed and Upcoming Projects

<details>
  <summary>📌 Accessing Bioinformatics Databases using Biopython </summary>

###

<details>
  <summary>✅ Sequence Alignment using NCBI BLAST </summary>

#### [View Documentation](https://github.com/sheetalreddy25/my-bio-hub/blob/5d455afccf9c6d19359b3acab38ab8a791e87fce/Project1_Documentation.md)

<details>
  <summary>🧬 Nucleotide BLAST (BLASTn) with NCBI </summary>

#### [**View Python Notebook**](https://github.com/sheetalreddy25/my-bio-hub/blob/main/nucleotide-blast-blastn-with-ncbi.ipynb)

#### Overview
This part of the project involves performing a Nucleotide BLAST (BLASTn) search using the TP53 gene sequence. BLASTn is used to compare a nucleotide sequence against the NCBI nucleotide database to identify homologous sequences.

#### Dataset
- The dataset used is the **TP53 gene sequence**, available at:  
  [NCBI TP53 Gene](https://www.ncbi.nlm.nih.gov/gene/7157)

</details>

<details>
  <summary>🧪 Protein BLAST (BLASTp) with NCBI </summary>

#### [**View Python Notebook**](https://github.com/sheetalreddy25/my-bio-hub/blob/main/protein-blast-blastp-with-ncbi.ipynb)

#### Overview
This part of the project involves performing a Protein BLAST (BLASTp) search using the translated TP53 protein sequence. BLASTp is used to compare an amino acid sequence against the NCBI protein database to identify homologous sequences.

#### Dataset
- The dataset used is the **TP53 protein sequence**, available at:  
  - [UniProt P04637](https://www.uniprot.org/uniprotkb/P04637/entry)  
  - [FASTA Download](https://rest.uniprot.org/uniprotkb/P04637.fasta)

</details>

</details>

---

<details>
  <summary>✅ Fetch PUBMED & Nucleotide Sequences using ENTREZ </summary>

#### [View Documentation](https://github.com/sheetalreddy25/my-bio-hub/blob/b156919fb7c4b28769c7950d4a931e999457fbc6/Project2_Documentation.md)

<details>
  <summary>📄 Fetch PUBMED using Entrez </summary>

#### [🧪 View Python Notebook](https://github.com/sheetalreddy25/my-bio-hub/blob/66597486962ebc7a87efb324f1a6583d19060029/fetch-pubmed-using-entrez.ipynb)

#### Overview
This part of the project involves retrieving data from the **PubMed** database using Biopython’s **Entrez API**. It includes searching for articles related to TP53 and formatting the results.

</details>

<details>
  <summary>🧬 Fetch Nucleotide Sequences using Entrez </summary>

#### [🧪 View Python Notebook](https://github.com/sheetalreddy25/my-bio-hub/blob/f9185416a09cd9799d7ce46e48aff519f8629798/fetch-nucleotide-sequences-using-entrez.ipynb)

#### Overview  
This part of the project demonstrates how to search for and retrieve **nucleotide sequences** from the **NCBI Nucleotide database** using Biopython’s Entrez module. It includes a gene-level search (TP53 in humans), and fetches records in both FASTA and GenBank formats.

</details>

</details>

---

<details>
  <summary>✅ Fetch Proteins from PDB </summary>
  
  #### [View Documentation](https://github.com/sheetalreddy25/my-bio-hub/blob/dd9c63885f64b056c95af264f31a4198930ccbec/Project3_Documentation.md)
  
  #### [🧪 View Python Notebook](https://github.com/sheetalreddy25/my-bio-hub/blob/d718147b7946c3870b87b37b2fcd502b7dad05bd/fetch-proteins-from-pdb.ipynb)

  #### Overview
  This part of the project involves retrieving and parsing protein structure data from the Protein Data Bank (PDB) using Biopython’s PDB module. It demonstrates downloading   the TP53 protein structure (PDB ID: 7BWN), extracting metadata, and summarizing chain and residue information.

</details>

---

###

<details><summary>✅ PROSITE & SCANPROSITE from EXPASY  </summary>

#### [View Documentation](https://github.com/sheetalreddy25/my-bio-hub/blob/c2e67298246dea404ac3827af32847497d1ee7ba/Project4_Documentation.md)

<details><summary>📄 Prosite Record Retrieval from ExPASy </summary>
  
#### [🧪 View Python Notebook](https://github.com/sheetalreddy25/my-bio-hub/blob/0af72729856097b01740643483c19bba64e59ef3/prosite-from-expasy.ipynb)

#### Overview
This part of the project focuses on **Data Retrieval and Parsing**. It uses Biopython's **ExPASy** and **Prosite** modules to fetch and parse the official PROSITE record (`PS00348`), which defines the conserved **p53 Family Signature**. This confirms the critical metadata, pattern syntax, and validation statistics before scanning.

</details>

<details><summary>🧬 ScanProsite & XML Parsing on TP53 Sequence </summary>
  
#### [🧪 View Python Notebook](https://github.com/sheetalreddy25/my-bio-hub/blob/78576c0f571991c2823b9a048dbe8d9e56e2c54f/scanprosite-from-expasy.ipynb)

#### Overview  
This part identifies functional domains in the human **TP53 protein sequence** (`P04637`). Due to current **incompatibilities between Biopython's high-level parsers and the modern ScanProsite API**, this project implements a custom solution: fetching raw XML data and using `xml.etree.ElementTree` to manually parse and locate the signature. This ensures accurate detection of the DNA-binding domain (found at positions 237-249) despite evolving server formats.

</details>

</details>

---

###

<details>
  <summary> ✅ Access KEGG Database  </summary>

  #### [View Documentation](https://github.com/sheetalreddy25/Bio-Python-Labs/blob/8d285390318cb367d042378a5516979fb564a456/Project5_Documentation.md)
  
  #### [🧪 View Python Notebook](https://github.com/sheetalreddy25/Bio-Python-Labs/blob/e9686318d4ab065ea55adb5facf97635ebafc3bf/access-kegg-database.ipynb)

  #### Overview
  This section demonstrates how to programmatically interface with the Kyoto Encyclopedia of Genes and Genomes (KEGG) database. Using Biopython's REST API, the project automates the retrieval of human TP53 gene data, performs custom string parsing to identify associated signaling pathways, and visualizes biological interaction maps directly within the workspace.
  
</details>

</details>

---

## 🔗 Connect with Me
- <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" alt="LinkedIn" width="16" style="vertical-align:middle;"/> [LinkedIn](https://www.linkedin.com/in/sheetalreddy25)
- 📧 [sheetal.reddy@g.austincc.edu](mailto:sheetal.reddy@g.austincc.edu)

