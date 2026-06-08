# Music Genre Classification

This repository contains the final project for music genre classification.

## Contents

This GitHub includes:

- The base code of the project
- The final presentation
- The final report

## Objective

The goal of this project is to classify songs by musical genre using different deep learning approaches.

## Dataset

The project is based on the **GTZAN** dataset, which contains 1000 audio clips of 30 seconds divided into 10 music genres.  
We use the GTZAN version distributed on Kaggle:

- Andrada Olteanu, “GTZAN Dataset – Music Genre Classification,” Kaggle, 2020. [web:203]

## Models Used

The project includes several approaches:

- MLP model with hand-crafted extracted features
- CNN model with spectrograms
- ResNet18 model with spectrograms (using `torchvision.models.resnet18`)

## Preprocessing

Different preprocessing steps were applied depending on the model:

- Tabular features were standardized with `StandardScaler` (scikit-learn)
- Spectrograms for the CNN were resized to the required input size
- ResNet used ImageNet-style normalization from `torchvision.transforms`

## How to Run

To run the project, simply open the notebook and execute the cells in order.  
No additional steps are needed.

## Main Libraries and Frameworks

This project relies on the following Python libraries:

- **PyTorch** (`torch`, `torch.nn`, `torch.optim`) for model implementation and training [web:217]  
- **Torchvision** (`torchvision.datasets`, `torchvision.transforms`, `torchvision.models.resnet18`) for data transforms and the ResNet18 backbone [web:170][web:214]  
- **scikit-learn** (`StandardScaler`, `LabelEncoder`, `train_test_split`, metrics) for preprocessing and evaluation  
- **Pandas** and **NumPy** for data handling and numerical operations  
- **Matplotlib** and **Seaborn** for visualizations  
- **tqdm** for training progress bars  
- **kagglehub** / Kaggle CLI for downloading the dataset

## Authors

Final project developed by Berta Miguel Ninou and Núria Esquius Bau, UPF engineering students.
