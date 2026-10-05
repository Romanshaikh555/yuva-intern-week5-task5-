# Week 5 Task: Deep Learning Application in Data Science

## Iris Flower Species Classification using Neural Network (TensorFlow / Keras)

### Project Overview
This project is part of the **Yuva Intern – Virtual Data Science Internship**.  
In this task I explored the fundamentals of deep learning and applied them to a multi-class classification
problem using a neural network built with **TensorFlow/Keras**.

The goal was to correctly classify Iris flower species (Setosa, Versicolor, Virginica)
based on four features: sepal length, sepal width, petal length, and petal width.

---

### Dataset
- **Name**: Iris Dataset  
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data)  
- **Samples**: 150 (50 per class)  
- **Features**: 4 continuous numerical features  
- **Target**: 3 classes (multi-class classification)

---

### Project Structure
```
├── Week5_DeepLearning_Iris_Classification.ipynb   # Main notebook (fully commented)
├── Week5_DeepLearning_Iris_Report.docx            # Detailed project report
└── README.md                                      # This file
```

---


### Model Architecture

| Layer            | Type     | Units / Rate | Activation |
|------------------|----------|--------------|------------|
| Input            | Input    | 4 features   | –          |
| Hidden Layer 1   | Dense    | 16           | ReLU       |
| Regularization   | Dropout  | 0.2          | –          |
| Hidden Layer 2   | Dense    | 8            | ReLU       |
| Output           | Dense    | 3            | Softmax    |

- **Optimizer**: Adam  
- **Loss**: Categorical Crossentropy  
- **Callbacks**: EarlyStopping + ReduceLROnPlateau  

---

### Results Summary
- Test Accuracy: **~93%**
- Iris-setosa was classified almost perfectly.
- Most residual errors occurred between Versicolor and Virginica (as expected from EDA).

---

### Key Steps Covered
1. Problem definition and dataset selection  
2. Exploratory Data Analysis (pair plots, correlation heatmap)  
3. Data preprocessing (label encoding, one-hot encoding, standardization)  
4. Neural network architecture design with justification  
5. Training with modern callbacks  
6. Evaluation using accuracy, precision, recall, F1-score and confusion matrix  
7. Critical analysis of challenges (overfitting, class overlap, small dataset) and solutions  

---

### Report
A detailed Word report (`Week5_DeepLearning_Iris_Report.docx`) is also included. It contains:
- Problem statement  
- Architecture diagrams  
- Training curves  
- Confusion matrix  
- Challenges faced and how they were solved  
- Critical insights  

---

### Tools & Libraries Used
- Python 3  
- TensorFlow / Keras  
- Pandas, NumPy  
- Matplotlib, Seaborn  

---

### Author
Created as part of **Yuva Intern – Virtual Data Science Internship**  
Week 5 Task: Deep Learning Application in Data Science
