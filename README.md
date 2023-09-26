# Software License Prediction with Support Vector Machine (SVM)

This project focuses on using a Support Vector Machine (SVM) to predict software license types based on various features. The dataset used for this project is loaded from a CSV file stored on Google Drive.

## Prerequisites

Before running the code, make sure you have the following libraries installed:

- Google Colab (if you're using Google Colab)
- pandas
- scikit-learn (for SVM and metrics)
- matplotlib
- seaborn (for visualization)

## Dataset

The dataset is loaded from the Google Drive path specified in the code (`file_path`). It contains information about software and its associated features, including the software name, company, and license type. The dataset is preprocessed as follows:

- Irrelevant columns ('About' and 'Link') are dropped.
- The 'License' column is converted to numerical labels.
- Categorical features are one-hot encoded.

## Training and Evaluation

The dataset is split into training and testing sets using `train_test_split` from scikit-learn. An SVM model with a linear kernel is initialized and trained on the training data. The following metrics are calculated on the test data:

- Accuracy
- Precision (weighted)
- Recall (weighted)

## Results and Visualization

The code generates the following results and visualizations:

- Model accuracy, precision, and recall are printed to the console.
- A classification report is generated, providing more detailed metrics.
- A confusion matrix is visualized using a heatmap, showing the predicted vs. actual license types.

## Model Saving

The trained SVM model is saved to a file using `joblib` and can be reused for making predictions on new data.

## Customization

You can customize this code by:

- Replacing the dataset file path (`file_path`) with your own dataset.
- Modifying the SVM model hyperparameters or kernel type.
- Adapting the code for other classification tasks or datasets.

Feel free to explore and adapt this project to suit your specific needs.

---

Enjoy using the Software License Prediction with SVM project!
