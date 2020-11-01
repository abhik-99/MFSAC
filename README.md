# MFSGC
Multi-Filtering Supervised Gene Clustering is a method which is designed to be used on Gene Expression Datasets for Filtering as well as Gene Augmentation and providing better genes for Cancer Classification.

## Setup.
The notebooks have been used on Google Colab. Please click on "Open in Colab" button at the top of each notebook. If you wish to use a local setup (not recommended), follow these step:- 
1. Install Python 3.8
2. Install Jupyter Notebook.
3. Start Jupyter notebook on your local setup and then open the notebooks.

## Datasets.
The datasets used for our proposed methods are:-
1. Leukemia 
2. Colon 
3. Prostate 
4. Lung 
5. RBreast
6. Breast 
7. MLL 
8. SRBCT

## Directory Structure


| Directory Name/Path | Significance |
|--------------|-------|
| Datasets | Contains all the datasets |
| Datasets/Original | Contains the Original Full Datasets |
| Datasets/Train-Test Split | Contains Random Splits of the Datasets |
| Datasets/Train-Test Split/<Dataset name> | Random split and MFSGC Results for that dataset |
| MFSGC Results | LOOCV Results of MFSGC |
| MFSGC Results/1200 Genes | Dataset-wise result taking top 1200 ranked/filtered genes |
| MFSGC Results/800 Genes | Dataset-wise result taking top 800 ranked/filtered genes |
| MFSGC Results/600 Genes | Dataset-wise result taking top 600 ranked/filtered genes |

## Usage
Run the notebooks (here we assume Google Colab). Start with **(Train)Multi-filtering Supervised Gene Clustering.**. This notebook provides the main proposed process. Run the cells which would -
1. Upload the datasets
2. Declare The functions
3. Form the Augmented Gene Clusters 
4. Run LOOCV Classification.
5. Save the Augmented Genes, the augmentation sequences and the results.

The above steps can be done on the whole dataset or the splits. Original Datasets as well as the train-test splits have been provided in the Repository. (refer to the section of *Directory Structure*). Notebooks starting with "Univariate" provide extra comparison with Univariate Filtering Methods and SGC. While the notebook "(Train)\_5_fold_Cross_Validation_on_MFSGC" builds on this notebook to provide 5 Fold Cross Validation Results.
