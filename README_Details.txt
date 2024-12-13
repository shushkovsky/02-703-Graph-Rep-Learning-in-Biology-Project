
# NR_AR Drugs

The dataset is designed to train a GNN model with the goal of identifying main drug components that activate the androgen receptor.

## Overview
- **Total Positive Cases**: 298
- **Total Negative Cases**: 6,626
- **Note**: The data had duplicate 'Main_Component' entries with approximately 78 positives and around 1,800 negatives. These duplicates were removed. ( Filter used: Function + Main_Component )

## Data Split
The data is divided into three sets as follows:
1. **Training Data**: Contains 70% of the data, balancing positive and negative cases. (4638 [0], 208 [1])
2. **Validation Data**: Contains 15% of the data. (994 [0], 45 [1])
3. **Test Data**: Contains 15% of the data. (994 [0], 45 [1])

## File Descriptions
- `Training_data_cleaned_split.xlsx`: Contains the training dataset.
- `Validation_data_cleaned_split.xlsx`: Contains the validation dataset.
- `Test_data_cleaned_split.xlsx`: Contains the test dataset.

## Column Descriptions
- **SMILE**: SMILES representation of the chemical structure.
- **ID**: Unique identifier for each compound.
- **Function**: Target variable indicating class; 0 for negative and 1 for positive.
- **DotCount**: Number of components - 1
- **Components**: Chemical components in the structure.
- **Total_Components_SaltRemoval**: Number of components after salt removal.
- **Main_Component**: Primary component in the chemical structure.

## Goal
The objective of this project is to identify the main component that could activate the receptor

---
