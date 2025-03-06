# Comparative Analysis of Multi-Omics Integration Using Graph Neural Networks for Cancer Classification

[![IEEE Access](https://img.shields.io/badge/IEEE_Access-10.1109/ACCESS.2025.3540769-brightgreen.svg)](https://doi.org/10.1109/ACCESS.2025.3540769)  [![arXiv](https://img.shields.io/badge/arXiv-2410.05325-b31b1b)](https://arxiv.org/abs/2410.05325)

Recent studies on integrating multiple omics data highlighted the potential to advance our understanding of the cancer disease process. Computational models based on graph neural networks and attention-based architectures have demonstrated promising results for cancer classification due to their ability to model complex relationships among biological entities. However, challenges related to addressing the high dimensionality and complexity in integrating multi-omics data, as well as in constructing graph structures that effectively capture the interactions between nodes, remain active areas of research. This study evaluates graph neural network architectures for multi-omics (MO) data integration based on graph-convolutional networks (GCN), graph-attention networks (GAT), and graph-transformer networks (GTN). Differential gene expression and LASSO (Least Absolute Shrinkage and Selection Operator) regression are employed for reducing the omics data dimensionality and feature selection; hence, the developed models are referred to as LASSO-MOGCN, LASSO-MOGAT, and LASSO-MOGTN. Graph structures constructed using sample correlation matrices and protein-protein interaction networks are investigated. Experimental validation is performed with a dataset of 8,464 samples from 31 cancer types and normal tissue, comprising messenger-RNA, micro-RNA, and DNA methylation data. The results show that the models integrating multi-omics data outperformed the models trained on single omics data, where LASSO-MOGAT achieved the best overall performance, with an accuracy of 95.9%. The findings also suggest that correlation-based graph structures enhance the models’ ability to identify shared cancer-specific signatures across patients in comparison to protein-protein interaction networks-based graph structures.

## 📁 Repository Organization
This repository is organized as follows:
- **Code/GAT_MultiOmicsData.ipynb**: contains codes for Graph Attention Network (GAT) for multi-omics data integration (mRNA, miRNA and DNA methylation), using the PPI (protein-protein interaction) graph structure.
- **Code/GCN_MultiOmicsData.ipynb**: contains codes for Graph Convolutional Network (GCN) for multi-omics data integration (mRNA, miRNA and DNA methylation), using the PPI (protein-protein interaction) graph structure.
- **Code/GTN_MultiOmicsData.ipynb**: contains codes for Graph Transformer Network (GTN) for multi-omics data integration (mRNA, miRNA and DNA methylation), using the PPI (protein-protein interaction) graph structure.

## 📊 Data
The provided file PPI.csv contains the information about the PPI (protein-protein interaction)network. 

## ▶️ Use
The codes are provided as Jupyter Notebook files. To reproduce the results, run the .ipynb files. 

## 🔨 Requirements
torch 2.0.1  
pandas 1.5.3  
numpy 1.23.5  
scikit-learn 1.2.2  

## 📖 Citation
If you use the codes or the methods in your work, please cite the following <a href="https://ieeexplore.ieee.org/abstract/document/10879447">article</a>:   

    @ARTICLE{Alharbi2025,
    TITLE={Comparative Analysis of Multi-Omics Integration Using Graph Neural Networks for Cancer Classification},
    AUTHOR={Alharbi, Fadi and Vakanski, Aleksandar and Zhang, Boyu and Elbashir, Murtada K. and Mohammed, Mohanad},
    JOURNAL = {IEEE Access},
    YEAR = {2025},
    VOLUME = {13},
    ISSUE = {},
    PAGES = {37724-37736},
    URL = {https://ieeexplore.ieee.org/abstract/document/10879447},
    DOI = {10.1109/ACCESS.2025.3540769}
    }

## 🚩 License
<a href="License - MIT.txt">MIT License</a>

## 👏 Acknowledgments
This work was supported by the National Institute of General Medical Sciences of the National Institutes of Health under Award P20GM104420.
 
## ✉️ Contact or Questions
<a href="https://www.webpages.uidaho.edu/vakanski/">A. Vakanski</a>, e-mail: vakanski at uidaho.edu

