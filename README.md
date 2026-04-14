#  Green Text Mining using Energy-Efficient Feature Representation and Adaptive Learning

##  Overview

This project implements an energy-efficient text mining framework by integrating feature optimization and adaptive learning techniques. It applies TF-IDF for compact feature representation and compares machine learning models to analyze performance and computational efficiency. The goal is to develop a sustainable text analytics system aligned with green data warehousing principles.


##  Objectives

* Perform sentiment analysis on textual data
* Reduce computational cost using efficient feature representation
* Compare baseline and adaptive machine learning models
* Evaluate performance using accuracy, F1-score, and execution time
* Simulate energy efficiency using execution time as a proxy

##  Dataset

* **Dataset:** IMDb Movie Review Dataset
* **Type:** Text (Sentiment Analysis)
* **Classes:** Positive (1), Negative (0)

##  Methodology

1. Data preprocessing and label conversion
2. Feature extraction using **TF-IDF**
3. Model implementation:

   * Naive Bayes (baseline)
   * SGD Classifier (incremental learning)
4. Model training and prediction
5. Performance evaluation and comparison


##  Models Used

### Naive Bayes

* Fast and simple baseline model
* Low computational cost
* Effective for text classification

###  SGD Classifier

* Supports incremental learning (`partial_fit`)
* Reduces retraining cost
* Scalable and energy-efficient


##  Evaluation Metrics

* Accuracy
* F1 Score
* Execution Time *(used as energy proxy)*

##  Results

| Model          | Accuracy | F1 Score | Execution Time |
| -------------- | -------- | -------- | -------------- |
| Naive Bayes    | 0.8517   | 0.8525   | 0.027 sec      |
| SGD Classifier | 0.8884   | 0.8922   | 0.33 sec       |

 Naive Bayes is faster, while SGD achieves higher accuracy and better scalability.


## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

##  How to Run

```bash
# Install dependencies
pip install pandas numpy scikit-learn
```

1. Download the IMDb dataset
2. Update the dataset path in the code
3. Run the Jupyter Notebook or Python script

##  Key Insights

* TF-IDF reduces storage and computation
* Incremental learning improves scalability
* Trade-off exists between speed and accuracy
* Energy efficiency can be approximated using execution time


##  Future Work

* Integrate real energy measurement tools (e.g., DBJoules)
* Extend to deep learning models
* Deploy on cloud platforms for large-scale processing



