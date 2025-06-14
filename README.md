📌 Introduction
The Resume Screening project processes and classifies resumes based on their content using machine learning models. It applies text cleaning, tokenization, vectorization, and model training to achieve high classification accuracy. The classifier helps in sorting resumes into categories like Data Science, HR, Software Engineer, etc.

📦 Installation
🔧 Prerequisites
Python 3.x

Jupyter Notebook / Google Colab
🧬 Dataset
| Column   | Description                          |
| -------- | ------------------------------------ |
| Resume   | Raw resume text                      |
| Category | Target label (e.g. Data Science, HR) |

🧹 Preprocessing Steps

1.Clean text (remove URLs, emojis, punctuation)
2.Tokenize and remove stopwords (using NLTK)
3.Encode labels using LabelEncoder
4.Vectorize text using TfidfVectorizer

🧠 Model Details
| Component     | Method                                    |
| ------------- | ----------------------------------------- |
| Vectorization | TF-IDF (max\_features=5000)               |
| Classifier    | K-Nearest Neighbors (KNN)                 |
| Strategy      | One-vs-Rest                               |
| Evaluation    | Accuracy, F1-score, classification report |

📊 Visualizations
✅ Category Distribution using CountPlot and Pie Chart

✅ WordCloud of most frequent resume terms

✅ Top Keywords used in resumes (after preprocessing)



🛠 Troubleshooting
Ensure NLTK data packages are downloaded.

Check if the dataset path is correctly specified.

Run on Google Colab for easy environment setup.