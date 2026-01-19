#  Fake News Detection Using Machine Learning

This project implements a **Fake News Detection System** using Machine Learning and Natural Language Processing (NLP). The system classifies news articles as **Fake** or **Real** based on their textual content.



---

##  Project Overview

With the rapid spread of misinformation on digital platforms, fake news detection has become an important problem. This project uses supervised machine learning algorithms to automatically identify fake news articles.

The workflow of the project includes:
- Loading and preprocessing the dataset
- Cleaning and transforming text data
- Feature extraction using TF-IDF
- Training multiple classification models
- Evaluating model performance
- Manual testing with user input

---

##  Technologies & Libraries Used

- Python  
- Pandas  
- NumPy  
- scikit-learn  
- Matplotlib  
- Seaborn  
- Regular Expressions (re)  
- Google Colab  

---

##  Dataset

The dataset is provided as a ZIP file and contains:
- `fake.csv` – Fake news articles  
- `true.csv` – Real news articles  

Each article is labeled as:
- `0` → Fake News  
- `1` → Real News  

Unnecessary columns such as `title`, `subject`, and `date` are removed before training.

---

##  Dataset Loading Note

Google Drive mounting could not be enabled during execution. Therefore, the dataset was **uploaded manually using `files.upload()`** and extracted locally from a ZIP file for further processing.

---

##  Data Preprocessing

Text preprocessing steps include:
- Converting text to lowercase
- Removing URLs and HTML tags
- Removing punctuation, digits, and special characters
- Cleaning noisy patterns using regular expressions

TF-IDF Vectorization is used to convert textual data into numerical features suitable for machine learning models.

---

##  Machine Learning Models Used

The following models are trained and evaluated:

- Logistic Regression  
- Decision Tree Classifier  
- Random Forest Classifier  



---

## Model Evaluation

The models are evaluated using:
- Accuracy score  
- Precision  
- Recall  
- F1-Score  

Evaluation results are displayed using `classification_report` from scikit-learn.

---

##  Manual News Testing

The project includes a manual testing feature where the user can input a custom news article. The system predicts whether the news is **Fake** or **Not Fake** using:
- Logistic Regression
- Decision Tree
- Random Forest

---

##  How to Run the Project

1. Upload the dataset ZIP file.
2. Extract the dataset.
3. Run the notebook cells sequentially.
4. Train the models.
5. Enter a news article when prompted to test manually.

---

##  Future Enhancements

- Implement Gradient Boosting / XGBoost
- Hyperparameter tuning
- Build a web interface using Flask or Streamlit
- Deploy the model as an API

---

