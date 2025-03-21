This repository contains datasets used in `AmpHGT: Expanding Prediction of Antimicrobial Activity in Peptides Containing Non-Canonical Amino Acids Using Multi-View Constrained Heterogeneous Graph Transformer`. 

Please download the data from https://drive.google.com/file/d/1Y4IdekvF3_GuM08Ce_pqFSYOz7x9IyoF/view?usp=sharing

Each dataset is provided as a .7z file, which store chemical structural information for each peptide.

### 1. `datasets_xuamp.7z`
- **Description**: This dataset contains peptides composed of canonical amino acids only. SMILES in each files is exactly correspond to the fasta sequences used by TP-LMMSG and XUAMP independent test set.

### 2. `datasets_AMPDiscover.7z`
- **Description**: This dataset contains peptides composed of canonical amino acids only. SMILES in each files is exactly correspond to the fasta sequences used by esm-AxP-GDL framework and external independent test set.

### 3. `datasets_ncaa.7z`
- **Description**: - **Description**: This dataset contains peptides composed of canonical amino acids and non-canonical amino acids. within the `ncaa_test_positive_2696.smi` and `ncaa_test_negative_2452.smi` correspond to the sequences of NCAA independent test set for 0-shot and jointing training benchmarking, the `ncaa_all_xuamp_train_negative_4635.smi`, `ncaa_all_xuamp_train_positive_4630.smi`, `ncaa_all_xuamp_val_positive_1246.fasta`, and `ncaa_all_xuamp_val_negative_1241.smi` correspond to the joint training dataset by merge NCAA overlap dataset and XUAMP training set.

## How to Access the Datasets

To extract the files, use the following command (on Linux, will require p7zip installed):

```bash
7z x <dataset_name>.7z
```

## License
Licensed under CC BY-NC 4.0.