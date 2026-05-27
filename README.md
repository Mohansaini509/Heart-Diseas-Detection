Heart Disease Detection System

A Machine Learning-based web application that predicts the likelihood of heart disease using patient health parameters. This project is built using Python, Flask, Scikit-learn, Pandas, and NumPy.

🚀 Project Overview

The Heart Disease Detection System is designed to help predict whether a patient is likely to have heart disease based on medical attributes such as age, blood pressure, cholesterol level, heart rate, and more.

The project uses the Gaussian Naive Bayes Machine Learning algorithm for prediction and provides a simple Flask-based web interface for user interaction.

📌 Features
Heart disease prediction using Machine Learning
User-friendly Flask web application
Data preprocessing using Label Encoding
Model training and evaluation
Real-time prediction through web form
CSV dataset support
🛠️ Technologies Used
Python
Flask
Pandas
NumPy
Scikit-learn
Pickle
HTML/CSS
📂 Project Structure
Heart-Disease-Detection/
│
├── app.py                # Flask web application
├── Main.py               # Model training script
├── hearts.csv            # Dataset file
├── model.pkl             # Trained machine learning model
├── templates/
│   └── index1.html       # Frontend HTML page
│
└── README.md
📊 Dataset Information

The dataset contains medical information of patients used to predict heart disease.

Input Features
Age
Sex
Chest Pain Type
Resting Blood Pressure
Cholesterol
Fasting Blood Sugar
Resting ECG
Maximum Heart Rate
Exercise Angina
Oldpeak
ST Slope
Target Variable
HeartDisease
1 → Heart Disease Present
0 → Normal Patient
⚙️ Machine Learning Workflow
1. Data Collection

The dataset is loaded using Pandas.

df = pd.read_csv('hearts.csv')
2. Data Preprocessing

Categorical values are converted into numerical values using LabelEncoder.

3. Train-Test Split

Dataset is divided into:

80% Training Data
20% Testing Data
4. Model Training

Gaussian Naive Bayes algorithm is used for training.

from sklearn.naive_bayes import GaussianNB
NB = GaussianNB()
NB.fit(x_train, y_train)
5. Model Evaluation

Accuracy is calculated using:

accuracy_score(y_test, y_pred)
6. Prediction

The trained model predicts whether the patient has heart disease or not.

🌐 Flask Application

The Flask application allows users to enter patient details through a web form and receive prediction results instantly.

Run Flask App
python app.py

Default Flask URL:

http://127.0.0.1:5000/
▶️ Installation Guide
Step 1: Clone Repository
git clone https://github.com/your-username/heart-disease-detection.git
Step 2: Navigate to Project Folder
cd heart-disease-detection
Step 3: Install Dependencies
pip install -r requirements.txt
Step 4: Run Training Script
python Main.py
Step 5: Run Flask Application
python app.py
📦 Required Libraries
Flask
numpy
pandas
scikit-learn
pickle-mixin
📈 Model Used
Gaussian Naive Bayes Classifier

Why GaussianNB?

Fast and efficient
Works well with small datasets
Good performance for classification problems
🧪 Sample Prediction
Input
Age = 29
Sex = Male
Chest Pain Type = 2
RestingBP = 100
Cholesterol = 106
FastingBS = 1
RestingECG = 2
MaxHR = 80
ExerciseAngina = 1
Oldpeak = 1
ST_Slope = 1
Output
The Patient Have Heart Disease, please consult the Doctor
📷 Future Improvements
Improve model accuracy using advanced algorithms
Add data visualization dashboard
Deploy project on cloud platforms
Add authentication system
Create responsive UI design
🤝 Contribution

Contributions are welcome. Feel free to fork the repository and improve the project.

📄 License

This project is developed for educational and learning purposes.

👨‍💻 Author

Mohan Saini
Aspiring Data Analyst & Machine Learning Enthusiast
