# Iris Flower Species Classification using SVM

This project applies a Machine Learning classification model to predict the species of an Iris flower based on its structural measurements. The project is implemented in Python using Google Colab and deployed on GitHub.

## 📊 Dataset Overview
The project uses the classic **Iris Dataset** from Kaggle. It contains 150 instances of Iris flowers across 3 distinct species:
* Iris-setosa
* Iris-versicolor
* Iris-virginica

Each flower is measured across 4 numerical features:
1.  Sepal Length (cm)
2.  Sepal Width (cm)
3.  Petal Length (cm)
4.  Petal Width (cm)

## 🤖 Why Support Vector Machine (SVM)?
For this dataset, **Support Vector Machine (SVM)** with a linear kernel was selected as the ideal algorithm. Because the dataset features clear, linearly separable boundaries between the species, SVM efficiently calculates optimal hyperplanes to maximize the margin between classes, yielding superior accuracy compared to complex neural networks.

## 🛠️ Project Workflow
1.  **Data Loading:** Reading the `IRIS.csv` file using Pandas.
2.  **Data Preprocessing:** * Encoded categorical labels (`species`) into numeric values using `LabelEncoder`.
    * Split the data into **80% Training** and **20% Testing** sets.
    * Standardized the features using `StandardScaler` (highly critical for SVM performance).
3.  **Model Training:** Trained a Scikit-Learn `SVC` classifier with a `linear` kernel.
4.  **Evaluation:** Analyzed performance using a Classification Report and a Confusion Matrix heatmap.

## 📈 Results & Performance
* **Model Accuracy:** The SVM model achieved an outstanding classification accuracy of **100%** on the test dataset.
* **Confusion Matrix:** Successfully predicted all target classes with zero misclassifications.

## 💻 Tech Stack Used
* **Environment:** Google Colab
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
