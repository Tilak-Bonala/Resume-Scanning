📌 Introduction
The Resume Screening project processes and classifies resumes based on their content using machine learning models. It applies text cleaning, tokenization, vectorization, and model training to achieve high classification accuracy. The classifier helps in sorting resumes into categories like Data Science, HR, Software Engineer, etc.

🚀 Usage
Load Dataset: Load the ResumeDataSet.csv containing resumes and their corresponding job categories.

Preprocess Text: Clean and tokenize the text, removing URLs, special characters, and stopwords.

EDA: Visualize distribution of job categories.

Feature Engineering: Apply TF-IDF vectorization.

Model Training: Train a KNeighborsClassifier using One-vs-Rest strategy.

Evaluation: Assess model performance using classification metrics.

✨ Features
Clean and preprocess resume text

Visualize resume category distribution

Extract most common keywords using WordCloud

Encode job categories for ML modeling

TF-IDF feature extraction

Train/test split for model evaluation

Model performance reporting with precision, recall, F1-score

📦 Dependencies
Key libraries used:

numpy, pandas

scikit-learn

matplotlib, seaborn

nltk

wordcloud

NLTK resources required:

python
Copy
Edit
nltk.download('punkt')
nltk.download('stopwords')
⚙️ Configuration
TF-IDF vectorizer configured with max_features=5000 and stop_words='english'

Train-test split ratio: 75% training, 25% testing

Classifier used: OneVsRestClassifier with KNeighborsClassifier

📊 Data Description
The dataset (ResumeDataSet.csv) contains:

Resume: Textual content of resumes

Category: Label indicating job domain (e.g., HR, Data Science)

The labels are encoded using LabelEncoder for model training.

🤖 Modeling
Model: K-Nearest Neighbors inside One-vs-Rest strategy

Vectorization: TF-IDF

Evaluation Metrics:

Accuracy on training and test sets

Precision, Recall, F1-score (using classification_report)

🛠 Troubleshooting
Ensure NLTK data packages are downloaded.

Check if the dataset path is correctly specified.

Run on Google Colab for easy environment setup.