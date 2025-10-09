# 🎯 End-to-End Machine Learning Project

An end-to-end **Machine Learning Pipeline** built using Python that automates the process of data ingestion, preprocessing, model training, and deployment through a Flask web app.

This project follows a modular and scalable architecture for building and deploying machine learning models efficiently.

---

## 🧩 Project Overview

This project demonstrates a complete machine learning workflow, from raw data to a deployable prediction service.  
It covers:
- Data ingestion from CSV files  
- Data cleaning and preprocessing  
- Feature engineering  
- Model training and evaluation  
- Saving artifacts (models, preprocessors, data splits)  
- Deploying a trained model via a Flask-based web interface

---

## 🏗️ Project Structure

```
mlproject/
│
├── app.py                     # Flask web application for model prediction
├── requirements.txt            # Python dependencies
├── setup.py                    # Project setup file for packaging
│
├── artifacts/                  # Stores intermediate and final ML artifacts
│   ├── data.csv
│   ├── train.csv
│   ├── test.csv
│   ├── model.pkl
│   └── preprocessor.pkl
│
├── notebook/                   # Jupyter notebooks for EDA and experiments
│   ├── 1. EDA STUDENT PERFORMANCE.ipynb
│   └── 2. MODEL TRAINING.ipynb
│
├── src/                        # Source code for the ML pipeline
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/               # Handles end-to-end pipeline execution
│   ├── utils.py
│   ├── logger.py
│   └── exception.py
│
└── README.md                   # Project documentation
```

---

## ⚙️ Installation

### 1️⃣ Clone the repository
```bash
git clone https://github.com/namansinghal1505/mlproject.git
cd mlproject
```

### 2️⃣ Create and activate a virtual environment
```bash
python -m venv venv
venv\Scripts\activate     # For Windows
source venv/bin/activate    # For macOS/Linux
```

### 3️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

---

## 🚀 Running the Application

### Run the training pipeline
This command will run the full machine learning pipeline — from data ingestion to model training.
```bash
python src/pipeline/train_pipeline.py
```

### Launch the Flask web app
Once the model is trained, start the Flask web app to serve predictions:
```bash
python app.py
```
Then, open your browser and go to:
```
http://127.0.0.1:5000/
```

---

## 🧠 Technologies Used

- **Python 3.8+**
- **Pandas**, **NumPy**, **Scikit-learn**
- **CatBoost**
- **Flask**
- **Matplotlib**, **Seaborn**
- **Logging & Exception Handling**

---

## 📊 Model Artifacts

All key outputs of the ML pipeline are saved under the `/artifacts` directory:
- `model.pkl` → trained machine learning model  
- `preprocessor.pkl` → preprocessing pipeline  
- `train.csv` / `test.csv` → training and test data splits  

---

## 🧪 Notebooks

Explore the `notebook/` folder to view:
- **EDA STUDENT PERFORMANCE.ipynb** → Data analysis and visualization  
- **MODEL TRAINING.ipynb** → Experimentation with model training and evaluation  

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!  
Feel free to open a pull request or issue.

---

## 🪪 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 👨‍💻 Author

**Naman Singhal**  
📧 [namansinghal1505@gmail.com](mailto:namansinghal1505@gmail.com)  
🔗 [GitHub Profile](https://github.com/namansinghal1505)

---
⭐ If you found this helpful, consider starring the repo to support the project!
