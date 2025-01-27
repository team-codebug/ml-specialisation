
# Machine Learning and Deep Learning Notes

---

## 1. Machine Learning (ML)

**Definition:**  
Machine Learning is the study and construction of programs that are not explicitly programmed but instead learn patterns by repeatedly observing data over time. These programs improve their performance as they are exposed to more data.

**Key Concept:**  
- The program identifies patterns from data rather than relying on explicit human instructions.  
- **Example:** Spam email classification.

**Diagram: Spam Classification Example**
```
Emails (Input) -> Machine Learning Program -> Predicted Label:
    - "This is spam"
    - "This is not spam"
```
The more labeled emails the program processes, the better it becomes at classification.

---

## 2. Machine Learning Terminology

1. **Features:**  
   Features are the attributes or characteristics of the data that are used to make predictions.  
   - **Example:** In a dataset of flowers, features could include:  
     ```
     Sepal length | Sepal width | Petal length | Petal width
     ```

2. **Target:**  
   The target is the specific column or output that the program is trying to predict.  
   - **Example:**  
     ```
     Target = Flower Species (e.g., Iris Setosa, Iris Virginica)
     ```

---

## 3. Types of Machine Learning

### Supervised Learning
- **Definition:** Involves a dataset with a target column (labeled data). The goal is to make predictions.  
- **Example:** Fraud detection, where the target is a label indicating whether a transaction is fraudulent or not.

**Diagram: Supervised Learning Workflow**
```
Data (Labeled) -> Train Algorithm -> Model -> Predictions
```

### Unsupervised Learning
- **Definition:** Works with datasets that do not have a target column. The goal is to find patterns or structure in the data.  
- **Example:** Customer segmentation in marketing, where the algorithm identifies groups of similar customers.

**Diagram: Unsupervised Learning Workflow**
```
Data (Unlabeled) -> Find Patterns -> Grouped Output
```

---

## 4. Summary Table

| **Category**           | **Definition**                                                             | **Examples**                                               |
|-------------------------|---------------------------------------------------------------------------|-----------------------------------------------------------|
| **Machine Learning (ML)** | Algorithms that improve as they process more data, learning patterns instead of explicit rules. | Spam detection, fraud detection.                         |
| **Features and Target** | Features are attributes of the data; the target is the column to predict. | Features: Sepal length; Target: Flower species.           |
| **Supervised Learning** | ML with labeled data, used for prediction.                               | Fraud detection, house price prediction.                  |
| **Unsupervised Learning** | ML with unlabeled data, used for pattern discovery.                      | Customer segmentation, clustering.                        |
| **Deep Learning (DL)**  | Advanced ML using deep neural networks to automatically learn features and make predictions. | Image recognition, voice assistants.                     |
| **Neural Network**      | A computational model mimicking the brain, with interconnected layers for feature extraction. | Input: Pixels; Output: "Cat" or "Dog".                   |

---

