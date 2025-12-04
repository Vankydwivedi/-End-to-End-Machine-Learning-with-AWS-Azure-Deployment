# 🎓 Student Performance Indicator — End-to-End ML Project

## 🚀 Overview
This project predicts student academic performance based on demographic and academic-related features using machine learning.
It demonstrates a complete ML lifecycle including data ingestion, validation, preprocessing, model training, evaluation, and prediction.

The target variable is the student's final score based on multiple factors such as gender, parental education, lunch type, and test preparation course.

---

## 📊 Dataset Description
Source: Kaggle – Student Performance in Exams  
Each row represents a student.

### Input Features:
- Gender  
- Race / Ethnicity  
- Parental level of education  
- Lunch type  
- Test preparation course  
- Reading score  
- Writing score  

### Target Variable:
- Math Score (predicted)

---

## 🧠 Project Workflow

```txt
Data Ingestion
     ↓
Data Validation
     ↓
Data Transformation (Encoding + Scaling)
     ↓
Model Training (Multiple Models)
     ↓
Model Evaluation
     ↓
Best Model Selection
     ↓
Prediction Pipeline
```

---

## 🧩 Project Structure

```
MLPROJECT-MAIN/
│
├── artifacts/
│   ├── model.pkl
│   ├── preprocessor.pkl
│
├── notebook/
│   ├── 1. EDA STUDENT PERFORMANCE.ipynb
│   ├── 2. MODEL TRAINING.ipynb
│
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   ├── model_trainer.py
│   │
│   ├── pipeline/
│   │   ├── train_pipeline.py
│   │   ├── predict_pipeline.py
│
├── train.csv
├── test.csv
├── requirements.txt
└── setup.py
```

---

## ⚙️ How to Run the Project

### 1. Clone the repository
```bash
git clone <your-repo-link>
cd MLPROJECT-MAIN
```

### 2. Create virtual environment
```bash
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate  # macOS/Linux
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Train the model
```bash
python src/pipeline/train_pipeline.py
```

### 5. Run prediction
```bash
python src/pipeline/predict_pipeline.py
```

---

## 📈 Results
The trained model achieves good predictive performance on unseen data.

(Add metrics such as R², RMSE, or MAE if needed.)

---

## 🧪 Notebooks

### EDA:
`1. EDA STUDENT PERFORMANCE.ipynb`  
- Feature distributions  
- Correlation analysis  
- Missing value handling  
- Visualization

### Model Training:
`2. MODEL TRAINING.ipynb`  
- Baseline models  
- Model comparison  
- Hyperparameter options  
- Final model selection

---

## 🛠 Tech Stack
- Python  
- Pandas, NumPy  
- scikit-learn  
- CatBoost (if used)  
- Logging module  

---

## 🔮 Future Enhancements
- Web UI for predictions  
- Model monitoring  
- Feature importance dashboard  
- CI/CD pipeline  
- Dockerization

---

## 📌 Disclaimer
This is an educational machine learning project focused on academic performance prediction.
It does not involve real-time student data or cloud deployment.
