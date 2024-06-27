# Computational Drug Discovery with ChEMBL Data

This repository provides scripts and instructions to download and preprocess biological activity data from the ChEMBL database for use in computational drug discovery. The dataset consists of compounds (molecules) tested for their biological activity against target organisms or proteins of interest.

# Table of Contents

1. Prerequisites
2. Setup
3. Downloading Data
4. Preprocessing Data
5. Usage
6. Contributing
7. License

# Prerequisites
Ensure you have the following software installed on your machine:

1. Python (>= 3.6)
2. wget (if you're using the command line to download data)
3. RDKit (for chemical informatics)
4. Pandas (for data manipulation)
5. NumPy (for numerical operations)

# Pre-processing the data
Preprocessing involves cleaning the data, handling missing values, and preparing it for analysis. 

# Understanding the Script

Input

"SMILES Strings": The script expects a CSV file (bioactivity_preprocessed_data.csv) with a column named canonical_smiles containing the SMILES strings of the compounds.

Output
"Lipinski's Descriptors": The script computes the following descriptors for each compound:
-Molecular Weight (MW)
-LogP (octanol-water partition coefficient)
-Number of Hydrogen Bond Donors (NumHDonors)
-Number of Hydrogen Bond Acceptors (NumHAcceptors)

"Script Explanation"
- Loading Data: The dataset is loaded into a Pandas DataFrame.
- Descriptor Calculation: Lipinski's descriptors are computed for each molecule.
- Computing Molecular Descriptors
- Normalizing Biological Activity Values
- Computing pIC50 Values
- Computing pIC50 Values

Contributing
Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.

