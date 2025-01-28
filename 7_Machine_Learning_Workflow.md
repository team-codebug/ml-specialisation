# Machine Learning Workflow and Vocabulary

---

## **Background and Tools**

Machine learning workflows typically require familiarity with specific tools and foundational concepts:

### **1. Prerequisites**
- **Programming Knowledge:**  
  - Familiarity with Python programming.  
  - Libraries such as **NumPy**, **Pandas**, and **Jupyter Notebooks** for data manipulation and visualization.
- **Basic Statistics:**  
  - Probability theory, calculating moments, and applying **Bayes' rule**.

### **2. Libraries and Tools Used**
The examples in this guide rely on:
- **NumPy:** Numerical computations.
- **Pandas:** Data manipulation and preprocessing.
- **Matplotlib/Seaborn:** Data visualization.
- **Scikit-Learn:** Machine learning models and preprocessing.
- **TensorFlow/Keras:** Building and training deep learning models.

---

## **Machine Learning Workflow**

The process of solving a problem with machine learning involves the following steps:

### **1. Problem Statement**
- Clearly define the problem you aim to solve.
- **Example:** Predicting house prices based on size, location, and number of rooms.

### **2. Data Collection**
- Identify and gather the data required to address the problem.
- **Example:** Collecting real estate data, such as historical house prices and property attributes.

### **3. Data Exploration and Preprocessing**
- Clean and prepare the data for the model.
  - Handle missing values.
  - Normalize or scale features.
  - Encode categorical variables.
- **Example:** Removing null values, standardizing house sizes, and encoding "City" into numeric values.

### **4. Modelling**
- Build a machine learning model to solve the problem.
  - Choose the appropriate algorithm (e.g., Linear Regression, Decision Trees, Neural Networks).
- **Example:** Training a regression model to predict house prices.

### **5. Validation**
- Evaluate the model's performance on unseen data.
  - Use metrics such as Mean Squared Error (MSE) or Accuracy, depending on the problem type.
- **Example:** Test the house price prediction model on a separate dataset to ensure accuracy.

### **6. Decision Making & Deployment**
- Communicate findings to stakeholders or deploy the model in production.
- **Example:** Integrating the prediction model into a real estate website.

---

## **Machine Learning Vocabulary**

### **1. Target**
- **Definition:** The category or value that we are trying to predict.
- **Example:** In a house price prediction model, the target is the price of the house.

### **2. Features**
- **Definition:** Properties of the data used for prediction (explanatory variables).
- **Example:** Size of the house, number of rooms, and location.

### **3. Example/Observation**
- **Definition:** A single data point within the dataset (represented by a row).
- **Example:** A single property with values:  
- Size: 1500 sq ft | Rooms: 3 | Location: New York | Price: $500,000

### **4. Label**
- **Definition:** The target value of a single data point.
- **Example:** For the observation above, the label is `$500,000`.

---

## **Real-World Example: Predicting House Prices**

| **Size (sq ft)** | **Rooms** | **Location**  | **Price**   |
|-------------------|-----------|---------------|-------------|
| 1500             | 3         | New York      | $500,000    |
| 2000             | 4         | San Francisco | $1,200,000  |
| 1200             | 2         | Chicago       | $350,000    |

### Vocabulary Applied:
- **Target:** Price  
- **Features:** Size, Rooms, Location  
- **Observation:** A single row (e.g., Size: 1500 sq ft, Rooms: 3, Location: New York, Price: $500,000).  
- **Label:** The price value ($500,000) for the observation.

---

## **References**

1. "Introduction to Machine Learning with Python" by Andreas C. Müller and Sarah Guido - [Book Link](https://www.oreilly.com/library/view/introduction-to-machine/9781449369880/)
2. Scikit-Learn Documentation: [Scikit-Learn API](https://scikit-learn.org/stable/)
3. TensorFlow Documentation: [TensorFlow API](https://www.tensorflow.org/)
4. "Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow" by Aurélien Géron - [Book Link](https://www.oreilly.com/library/view/hands-on-machine-learning/9781492032632/)
5. Pandas Official Documentation: [Pandas API](https://pandas.pydata.org/)

---

This document provides a structured overview of the machine learning workflow, vocabulary, and practical examples to help you get started with machine learning projects.
