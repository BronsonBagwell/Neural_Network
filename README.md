# Neural Network
Neural network model for predicting graduate admission using 1, 2, and 3 hidden layer architectures.

## Overview
This project builds neural networks with varying architectures (1, 2, and 3 hidden layers) to predict graduate admission outcomes. The analysis explores how normalization and model architecture affect prediction accuracy on structured admissions data.

## Dataset
- **Source:** Graduate Admission dataset
- **Key variables:** GRE Score, TOEFL Score, University Rating, SOP, LOR, CGPA, Research Experience

## Methods
- Min-Max normalization of all numeric features
- 80/20 train-test split for model evaluation
- Neural networks with 1, 2, and 3 hidden layers using the `neuralnet` package
- Model comparison across architectures

## Key Findings
- CGPA, GRE Score, and SOP were identified as the top predictors of admission
- Neural network required careful normalization to achieve stable training
- Comparing hidden layer architectures revealed trade-offs between complexity and performance

## Tools & Libraries
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=R&logoColor=white)
![neuralnet](https://img.shields.io/badge/neuralnet-276DC3?style=flat-square&logo=r&logoColor=white)
![caret](https://img.shields.io/badge/caret-276DC3?style=flat-square&logo=r&logoColor=white)

## How to Run
1. Clone the repository: `git clone https://github.com/BronsonBagwell/Neural_Network.git`
2. Open the HTML file in a browser, or run the R Markdown file in RStudio
3. Required packages: `neuralnet`, `caret`
