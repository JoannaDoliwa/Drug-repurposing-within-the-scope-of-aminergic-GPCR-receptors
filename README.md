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
- os (standard library)

## Project Structure
- `projekt_zaliczeniowy_mldd.ipynb`: Main Jupyter Notebook containing the entire workflow of the project.
- `serotoninergic_config/`: 
- `serotoninergic_pdb/`: 
- `serotoninergic_pdbqt/`: 
- `GPCRdb_alignment_aminergic_binding_site.csv`:
- `serotoninergic_drugs.csv`: 
- `serotoninergic_ligands_table.csv`: 

## Results
The results of the docking simulations and model predictions will be displayed within the notebook. Outputs include binding affinity scores and auxiliary data from the `dockstring` library.

## License
This project is licensed under the MIT License. 
