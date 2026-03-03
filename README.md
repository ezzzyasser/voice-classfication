# Gender Recognition by Voice and Speech Analysis
This project utilizes machine learning and acoustic analysis to identify the gender (Male or Female) of a speaker based on their voice properties. The system analyzes frequency and spectral characteristics to build a robust classification model.

## 🚀 Project Overview
Voice recognition technology is a key component of modern AI interfaces. This project demonstrates how specialized acoustic features—such as fundamental frequency and spectral flatness—can be used to distinguish between male and female voices with high precision.

## 🛠️ Technical Workflow

**Acoustic Analysis**: The dataset consists of 3,168 samples pre-processed with an analyzed frequency range of 0Hz–280Hz (the human vocal range).
**Feature Engineering**: The models utilize **20 distinct acoustic features**, including:
`meanfun`: Average fundamental frequency (a key differentiator).
`sd`: Standard deviation of frequency.
`IQR`: Interquartile range.
`sp.ent`: Spectral entropy.


**Exploratory Data Analysis (EDA)**:
Utilized **Kernel Density Estimation (KDE)** to visualize feature distributions.
Generated **Correlation Matrices** and scatter plots to identify highly dependent acoustic traits.

**Model Selection**: Evaluated three classification algorithms to determine the most effective approach for gender detection.

## 🤖 Models & Performance
The project compares three main classification models:

**Decision Tree**: (Best Performer) Achieved the highest accuracy, precision, and F1-score.
**K-Nearest Neighbors (KNN)**: Evaluated for its effectiveness in feature-space clustering.
**Logistic Regression**: Implemented as a baseline statistical classification model.

**Analysis**: The **Decision Tree** was selected as the final model due to its superior **AUC (Area Under Curve)** and perfect prediction rate as shown in the confusion matrix.


## 🧰 Tech Stack

* **Python**: Primary programming language.
* **Pandas & NumPy**: Data processing and analysis.
* **Matplotlib & Seaborn**: Advanced statistical visualizations.
* **Scikit-Learn**: Machine learning implementation and performance metrics (ROC, AUC, Confusion Matrix).
