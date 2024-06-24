# Project Title: Drug repurposing within the scope of aminergic GPCR receptors

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Project Structure](#project-structure)
- [Results](#results)
- [License](#license)

## Introduction
This project focuses on the application of chemiinformatics techniques to drug docking simulations and computing similarity scores between amino acid binding site serotoninergic GPCR receptor structures. Using the `dockstring` library, the project aims to predict the binding affinity of approved or in-clinical-trials to serotoninergic GPCR receptors other than for the one for which the drug has been approved for. Finally, the Pearson correlation coefficient and p-value are calculated for the relationship (for a given drug) between the docking scores and receptor similarity to the receptor for which the drug was initially designed for. Statistically significant negative correlation would indicate that the possibility for repurposing the given drug is greater for structurally similar receptors.    
The notebook explores the data preprocessing, model training, evaluation, and docking process.

## Prerequisites
- Python 3.x
- Jupyter Notebook
- Basic knowledge of cheminformatics and drug discovery.


## Usage
1. Launch Jupyter Notebook:
   ```sh
   jupyter notebook
   ```

2. Open the `projekt_zaliczeniowy_mldd.ipynb` notebook and execute the cells to run the analysis.

## Dependencies
The project requires the following Python libraries:  
- pandas
- numpy
- biopython
- rdkit
- dockstring
- matplotlib

## Project Structure
- `projekt_zaliczeniowy_mldd.ipynb`: Main Jupyter Notebook containing the entire workflow of the project.
- `serotoninergic_config/`: This directory contains configuration files for docking based on the calculated center and dimensions of the serotoninergic GPCR receptors.
- `serotoninergic_pdb/`: This directory contains PDB (Protein Data Bank) files of serotoninergic receptors. PDB files provide detailed three-dimensional structures of proteins, which are essential for conducting molecular docking studies to understand how ligands bind to these receptors.
- `serotoninergic_pdbqt/`: This directory contains PDBQT files, which are modified PDB files including charges and atom types necessary for the docking simulations. These files are used as input for molecular docking software such as AutoDock Vina.
- `GPCRdb_alignment_aminergic_binding_site.csv`: This file contains alignment data of the aminergic binding sites of G protein-coupled receptors (GPCRs) from the GPCRdb database. The alignment helps in understanding the conserved regions across different GPCRs, which is crucial for comparative modeling and designing ligands targeting these receptors.
- `serotoninergic_drugs.csv`: This file contains a list of serotoninergic drugs along with relevant information such as their chemical names, molecular formulas, and potentially their therapeutic uses. 
- `serotoninergic_ligands_table.csv`: This file contains detailed information about various ligands that interact with serotoninergic receptors and most importantly their Smiles structures.

## Results
Unfortunately, no statistically significant correlation was found between docking and similarity scores for any one of the examined drugs (p-value > 0.05 for all calculations). Example plot for 5HT-1A antagonist and smooth mustle relaxant alverine provided below.



![docking_scores_vs_similarity_5ht1a_row_alverine](https://github.com/JoannaDoliwa/Drug-repurposing-within-the-scope-of-aminergic-GPCR-receptors/assets/125126159/ed77200a-f02b-40bc-b2e4-6bc38e160e2e)



## License
This project is licensed under the MIT License. 
