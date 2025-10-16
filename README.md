

---

## 🧠 Coding Fingerprint

**Semester 5 — Machine Learning Project**
**Team:** 29(Bilal,Mayan)

---

### 🚀 Project Overview

This project identifies a programmer’s **unique coding fingerprint** — the hidden patterns and styles that define how they write code.
By analyzing structural and stylistic features (variable naming, indentation, function patterns, etc.), the system predicts:

* 🏆 **Competitive Programming Rank** (e.g., Newbie, Expert, Master)
* 🌍 **Country/Region** of the user

The idea explores the **intersection between machine learning and software behavior analysis** — showing how a coder’s personal traits reflect in their code.

---

### 🧩 Key Features

* 🧹 **Data Cleaning & Preprocessing:** Removes noise and standardizes code samples.
* 🤖 **ML Model Training:** Predicts programmer’s rank and country.
* 📊 **Feature Engineering:** Extracts meaningful features (tokens, syntax structures, indentation depth).
* 💻 **Frontend (Streamlit):** Upload or paste code and view prediction results instantly.
* 🔙 **Backend (Flask):** Handles prediction logic and model inference via API.
* 📁 **Dataset:** 25,000+ code samples from competitive programmers on **Codeforces**.

---

### 🏗️ Project Architecture

```
Coding-Fingerprint/
│
├── backend.py                 # Flask backend API
├── frontend.py                # Streamlit frontend
├── data_creation.py           # Data generation and preprocessing script
├── data_cleaning.ipynb        # Notebook for cleaning and filtering data
├── codeforces_prediction.ipynb# Model training and evaluation
├── enhanced_codeforces_dataset.csv # Cleaned dataset
├── codeforces_filtered_users.csv   # Filtered Codeforces users data
│
├── pyproject.toml             # Project dependencies (Poetry)
├── LICENSE                    # Apache 2.0 License
├── README.md                  # Documentation
└── uv.lock                    # Dependency lock file
```

---

### ⚙️ Tech Stack

| Layer               | Technology                                           |
| ------------------- | ---------------------------------------------------- |
| **Language**        | Python 3.10                                          |
| **Frontend**        | Streamlit                                            |
| **Backend**         | Flask                                                |
| **Libraries**       | Scikit-learn, Pandas, NumPy, TfidfVectorizer, Pickle |
| **Dataset Source**  | Codeforces user profiles and code submissions        |
| **Version Control** | Git + GitHub                                         |

---

### 🧠 Model Pipeline

1. **Data Collection:** Scrape or import user code, rank, and country from Codeforces.
2. **Feature Extraction:** Apply tokenization, TF-IDF, and syntactic feature extraction.
3. **Training:** Train models (Logistic Regression, Random Forest, or SVM).
4. **Evaluation:** Measure accuracy and F1-score.
5. **Deployment:** Serve model through Flask and visualize in Streamlit.

---

### 🧪 How to Run Locally

#### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/Coding-Fingerprint.git
cd Coding-Fingerprint
```

#### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate     # Mac/Linux
venv\Scripts\activate        # Windows
```

#### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

#### 4️⃣ Run Backend (Flask)

```bash
python backend.py
```

#### 5️⃣ Run Frontend (Streamlit)

```bash
streamlit run frontend.py
```

#### 6️⃣ Use the App

* Paste your C++/Python code
* Click **Predict** to get your **Rank** and **Country**

---

### 📊 Example Output

| Input Code               | Predicted Rank   | Predicted Country |
| ------------------------ | ---------------- | ----------------- |
| Simple sorting algorithm | Expert           | India             |
| Dynamic programming code | Candidate Master | Japan             |

---

### 📁 Dataset Description

| Column         | Description                  |
| -------------- | ---------------------------- |
| `user_handle`  | Codeforces username          |
| `rank`         | Competitive programming rank |
| `country`      | User country                 |
| `code_snippet` | Source code collected        |
| `tokens`       | Extracted code features      |

---

### 📈 Results

| Model               | Accuracy | F1 Score |
| ------------------- | -------- | -------- |
| Logistic Regression | 86%      | 0.84     |
| Random Forest       | 89%      | 0.87     |
| SVM                 | 88%      | 0.86     |

---

### 🌟 Future Enhancements

* Add **GitHub profile integration** for broader code data.
* Introduce **neural network models** (RNN/BERT-based).
* Enhance **UI/UX** for better visualization of feature importance.
* Extend predictions to **experience level** and **domain expertise**.

---

### 👨‍💻 Authors

* **Mohammed Bilal** – ML & Backend
* **Team Bilalinbytes** – Data collection & Frontend

---

### 📜 License

Licensed under the **Apache License 2.0**.
You are free to use, modify, and distribute this project with attribution.

---


