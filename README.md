# Credit Card Fraud Detection <img src="https://www.shutterstock.com/image-vector/goblins-pot-goldvector-illustration-simple-260nw-1756871615.jpg" alt="Image" width="100"/>

This project aims to analyse and compare the performance of different machine learning classifiers in detecting credit card fraud. The dataset used to train and test the models in this project is the [Credit Card Fraud Detection dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud) from Kaggle.

## Evaluation Metrics

Considering the nature of the classification problem as well as the large class imbalance in the dataset, the project proposes a custom evaluation metric which heavily penalizes false negatives.

The rationale behind this approach is the assumption that the cost of missing a fraudulent transaction is much higher than the cost of flagging a legitimate transaction for review. Furthermore, due to the miniscule size of the share of fraudulent transactions it is generally unavoidable for any high-recall model to also have a notably large number of false positives.


## Tested Models

The following classifiers were tested in this project:
- `Logistic Regression`
- `Random Forest`
- `Adaptive Boosting`
- `K-Nearest Neighbors`
- `Voting Classifier` (Logistic Regression, Random Forest, K-Nearest Neighbors)

In addition a simple neural network was trained on the dataset and compared to the performance of the traditional classifiers.

## Usage and Dependencies

To run the project simply clone the repository, create a virtual environment from the `requirements.txt` file and run all cells in the Jupyter notebook.

The project utilizes the following libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `imblearn`
- `tensorflow`

## Authors

This project was created by [Krzysztof Kalita](https://github.com/k-kalita) and [Mateusz Kadula](https://github.com/m-kadula) as part of the entry to machine learning course at the *Jagiellonian University*.