# 🧬 Identification of Regulatory Hub Genes in Alzheimer's Disease Using Transcriptomic and Network Analysis

## 📖 Overview

Alzheimer's disease (AD) is a progressive neurodegenerative disorder characterized by memory loss, cognitive decline, and synaptic dysfunction. Although numerous genes have been associated with AD, the key regulatory mechanisms underlying disease progression remain incompletely understood.

This project integrates **transcriptomic analysis** with **Protein–Protein Interaction (PPI) network analysis** to identify regulatory hub genes associated with Alzheimer's disease. Differential gene expression analysis was performed using the **GSE122063** RNA-seq dataset from the Gene Expression Omnibus (GEO), followed by visualization, network construction, and hub gene identification.

---

## 🎯 Objectives

- Identify Differentially Expressed Genes (DEGs) between Alzheimer's disease and healthy control samples.
- Analyze transcriptomic differences using statistical and dimensionality reduction techniques.
- Visualize significant gene expression changes using Volcano Plot, Heatmap, and PCA.
- Construct a Protein–Protein Interaction (PPI) network using STRING.
- Identify regulatory hub genes through network centrality analysis.
- Interpret hub genes in the context of neurodegeneration, synaptic dysfunction, and neuroinflammation.

---

## 📂 Dataset

| Attribute | Details |
|----------|---------|
| Dataset | GSE122063 |
| Database | NCBI Gene Expression Omnibus (GEO) |
| Platform | GPL16699 |
| Disease | Alzheimer's Disease |
| Samples | 100 Brain Tissue Samples |
| Alzheimer's Samples | 56 |
| Control Samples | 44 |

---

## 🛠 Technologies Used

### Programming

- Python
- Google Colab

### Libraries

- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Scikit-learn
- GEOparse
- MyGene

### Bioinformatics Tools

- GEO Database
- STRING Database
- Cytoscape

---

# 🔬 Methodology

```text
             GEO Dataset (GSE122063)
                       │
                       ▼
            Data Collection & Preprocessing
                       │
                       ▼
            Differential Gene Expression Analysis
                       │
                       ▼
       Significant DEGs (log₂FC & p-value filtering)
                       │
          ┌────────────┼─────────────┐
          ▼            ▼             ▼
    Volcano Plot   Heatmap          PCA
                       │
                       ▼
           Gene Annotation & Mapping
                       │
                       ▼
      STRING Protein–Protein Interaction Network
                       │
                       ▼
        Network Centrality Analysis (Cytoscape)
                       │
                       ▼
      Identification of Regulatory Hub Genes
                       │
                       ▼
      Biological Interpretation of Hub Genes
```

---

# 📊 Differential Gene Expression Analysis

The RNA-seq expression profiles were statistically analyzed to identify Differentially Expressed Genes (DEGs).

### Criteria

- p-value < 0.05
- |log₂ Fold Change| > 1

Statistically significant genes were selected for downstream analysis and network construction.

---

# 📈 Data Visualization

The project includes multiple visualization techniques to understand transcriptomic alterations.

### ✔ Volcano Plot

- Displays significantly upregulated and downregulated genes.
- Highlights statistically significant DEGs.

### ✔ Heatmap

- Generated using the **Top 50 Differentially Expressed Genes**.
- Clearly distinguishes Alzheimer's disease and healthy control samples.
- Red indicates high expression.
- Blue indicates low expression.

### ✔ Principal Component Analysis (PCA)

PCA demonstrates clear separation between disease and control samples.

- PC1 explains **37.6%** variance.
- PC2 explains **11.3%** variance.

The clustering validates the biological distinction between Alzheimer's disease and healthy controls.

---

# 🧬 Protein–Protein Interaction (PPI) Network Analysis

Significant DEGs were imported into the STRING database to construct a Protein–Protein Interaction network.

Network topology analysis was performed to identify highly connected regulatory genes responsible for disease progression.

---

# ⭐ Hub Gene Identification

Network centrality analysis identified **15 regulatory hub genes** associated with Alzheimer's disease.

### Major Hub Genes

- SNAP25
- GFAP
- BDNF
- CALB1
- SST
- SLC17A6
- GAD1
- GAD2

### Biological Significance

These hub genes are associated with

- Synaptic dysfunction
- Neuroinflammation
- Neuronal signaling imbalance
- Neurodegeneration

Degree centrality analysis identified **SNAP25** as the most connected regulatory hub gene within the interaction network.

---

# 📌 Key Findings

- Successfully identified Differentially Expressed Genes from Alzheimer's transcriptomic data.
- Generated Volcano Plot, Heatmap, and PCA for transcriptomic visualization.
- Constructed Protein–Protein Interaction network using STRING.
- Identified 15 highly connected regulatory hub genes.
- SNAP25 emerged as the strongest hub gene based on degree centrality.
- The identified genes are strongly associated with synaptic signaling and neurodegeneration.

---

# 📁 Project Structure

```
Alzheimers-Hub-Gene-Analysis/
│
├── data/
│
├── notebooks/
│   └── Alzheimer_DEG_GSE122063.ipynb
│
├── results/
│   ├── VolcanoPlot.png
│   ├── Heatmap.png
│   ├── PCA.png
│   ├── STRING_Network.png
│   ├── Cytoscape_Network.png
│   └── DEG_Results.csv
│
├── README.md
└── requirements.txt
```

---

# 📷 Results

✔ Differential Gene Expression Analysis

✔ Volcano Plot

✔ Heatmap of Top DEGs

✔ Principal Component Analysis (PCA)

✔ STRING Protein Interaction Network

✔ Cytoscape Network Visualization

✔ Regulatory Hub Gene Identification

---

# 🚀 Future Scope

- Gene Ontology (GO) enrichment analysis
- KEGG pathway enrichment
- Functional validation of hub genes
- Machine learning-based biomarker prediction
- Multi-omics integration
- Experimental validation using clinical datasets

---

# 👨‍💻 Author

**Siddhesh Eknath Doke**
