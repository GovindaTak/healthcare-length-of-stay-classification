# healthcare-length-of-stay-classification
A deep learning project predicting the length of stay (LOS) for patients in hospitals using a multiclass classification approach. The project leverages PyTorch to implement a robust neural network model with advanced regularization techniques, aiming to optimize healthcare resource allocation.
------------------

### Repository Name  
`healthcare-length-of-stay-classification`

---

### Repository Description  
A deep learning project aimed at predicting hospital patient length of stay (LOS) for efficient healthcare management. The model leverages advanced preprocessing, visualization, and a fully connected neural network to classify LOS into 11 distinct categories, optimizing hospital logistics and patient management.

---

## Overview  
This project focuses on predicting the **Length of Stay (LOS)** for hospital patients as part of healthcare management. By leveraging **deep learning techniques**, the model classifies patients into 11 distinct categories based on their expected LOS. Accurate predictions help optimize healthcare logistics, improve patient management, and reduce operational inefficiencies.

---

## Problem Statement  
The **COVID-19 pandemic** has highlighted the critical need for efficient healthcare management. A key metric for hospitals is **Length of Stay (LOS)**, which impacts room allocation, staff management, and infection control.  

This project addresses the problem by building a multiclass classification model to predict LOS based on patient demographics, hospital details, and admission information. The LOS categories range from **0-10 days** to **100+ days**.

---

## Features

### **Data Preprocessing**  
- Handled missing values by dropping rows with <1.5% of total missing values.
- Dropped irrelevant columns (`case_id`, `patientid`) to avoid data leakage.
- Applied **One-Hot Encoding** and **Standard Scaling** to categorical and numerical features, respectively.

### **Data Visualization**  
- Analyzed data distribution and relationships using heatmaps and distribution plots.
- Verified no high correlation between features to prevent multicollinearity.

### **Neural Network Architecture**  
- Built a fully connected neural network with:
  - **Input Layer**: Standardized and encoded features.
  - **Hidden Layers**: LayerNorm, Dropout, and LeakyReLU activation for stability.
  - **Output Layer**: 11 neurons for multiclass classification.
- Trained the model using the **Adam Optimizer** and **CrossEntropyLoss**.

### **Regularization and Optimization**  
- Used **Dropout** and **Layer Normalization** for generalization.
- Early stopping with a patience level of 50 epochs to prevent overfitting.

### **Evaluation Metrics**  
- Accuracy: Measured overall model performance.
- Loss Curves: Analyzed training vs testing loss for convergence.

---

## Technologies Used  
- **Deep Learning Framework**: PyTorch  
- **Data Manipulation**: Pandas, NumPy  
- **Visualization**: Matplotlib, Seaborn  
- **Optimization**: Adam, Dropout, LayerNorm  

---

## Results and Insights  
### Key Metrics:  
- **Training Accuracy**: ~43.1%  
- **Testing Accuracy**: ~41.9%  

### Insights:  
- Early stopping effectively prevented overfitting.
- Features like **Type of Admission** and **Severity of Illness** showed strong predictive capabilities.
- Balancing the dataset or employing advanced techniques like ensemble models could improve performance further.

---

## How to Use  

1. **Clone the Repository**:  
   ```bash
   git clone https://github.com/GovindaTak/healthcare-length-of-stay-classification.git
   ```
2. **Navigate to the Directory**:  
   ```bash
   cd healthcare-length-of-stay-classification
   ```
3. **Install Dependencies**:  
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the Jupyter Notebook**:  
   ```bash
   jupyter notebook HealthHabit_LOS_Classification.ipynb
   ```

---

## Future Work  
- **Data Augmentation**: Explore techniques to handle class imbalance.  
- **Feature Engineering**: Derive new features like comorbidity scores.  
- **Advanced Models**: Use ensemble learning or transfer learning for improved accuracy.

---

## License  
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact  
For inquiries or collaborations, feel free to reach out at govindatak19@gmail.com.  
Explore more projects on my [GitHub](https://github.com/GovindaTak).
```
