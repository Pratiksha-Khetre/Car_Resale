🚗 Car Resale Price Prediction

An AI/ML-based project that predicts the resale price of used cars based on various factors such as brand, model, age, kilometers driven, fuel type, transmission, ownership history, and accident history.

The main objective of this project is to build a machine learning model that estimates the market resale value of a used car using historical car sales data.

🎯 Project Objectives

- Predict the resale price of used cars.
- Understand how different car features influence resale value.
- Perform data preprocessing and feature engineering.
- Experiment with different machine learning algorithms.
- Evaluate and compare model performance.

📊 Dataset Information

The dataset contains approximately 140,904 records with the following attributes:

Feature| Description
Brand| Manufacturer of the car
Model Name| Car model
Model Variant| Specific variant of the car
Car Type| SUV, Sedan, MPV, Luxury, etc.
Transmission| Manual or Automatic
Fuel Type| Petrol, Diesel, Electric, Hybrid
Year| Manufacturing year
Kilometers| Total distance driven
Owner| Number of previous owners
State| Location of the car
Accidental| Accident history
Price| Resale price (Target Variable)

🛠️ Technologies & Libraries

- Python – Programming language
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Matplotlib & Seaborn – Data visualization
- Scikit-learn – Machine learning and preprocessing

Machine Learning Algorithms

- Linear Regression
- Random Forest Regressor
- XGBoost Regressor
- CatBoost (planned experimentation)

⚙️ Project Workflow

1. Data Loading & Exploration

- Loaded the dataset using Pandas.
- Examined dataset structure, data types, and statistical information.
- Checked for missing values and inconsistencies.

2. Feature Engineering

Created additional features to improve prediction:

- Age: Current Year - Manufacturing Year
- Km_Per_yr: Total Kilometers / Car Age

3. Data Preprocessing

Applied different preprocessing techniques:

- Binary encoding for accidental history.
- One-Hot Encoding for categorical features such as Owner and Fuel Type.
- Mean (Target) Encoding for Brand.
- Feature scaling using StandardScaler where appropriate.

4. Model Training

Started with Linear Regression as the baseline model.

The model was trained using a train-test split to evaluate its performance on unseen data.

5. Model Evaluation

The following evaluation metrics are used:

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

📈 Model Improvement Strategy

Rather than directly implementing complex algorithms, the project follows an incremental learning approach:

1. Start with a basic Linear Regression model.
2. Train using minimal features.
3. Add new features one by one.
4. Observe changes in model performance.
5. Experiment with different encoding techniques.
6. Explore non-linear machine learning algorithms.
7. Compare models to identify the best-performing approach.

📂 Project Structure

Car-Resale-Price-Prediction/
│
├── Dataset/
│   └── Car Sell Dataset.csv
│
├── Model/
│   ├── Model1.py
│   └── Model2.py
│
├── README.md
│
└── requirements.txt

🚀 Installation & Execution

1. Clone the repository

git clone YOUR_GITHUB_REPOSITORY_URL

2. Navigate to the project directory

cd Car-Resale-Price-Prediction

3. Install dependencies

pip install pandas numpy matplotlib seaborn scikit-learn

4. Run the model

python Model/Model2.py

🔮 Future Enhancements

The project is currently focused on resale price prediction. Future improvements include:

- Car Condition Detection: Analyze uploaded car images using computer vision to estimate vehicle condition.
- VIN & RC Analysis: Explore extracting vehicle information using Vehicle Identification Numbers (VIN) and Registration Certificates (RC).
- Car Comparison: Compare multiple cars based on price, mileage, specifications, and resale value.
- Advanced ML Models: Experiment with Random Forest, Gradient Boosting, XGBoost, and CatBoost.
- Web Application: Develop a user-friendly interface for car price prediction.
- Recommendation System: Recommend suitable used cars based on user preferences and budget.

👩‍💻 Author

Developed as a hands-on Machine Learning project to explore data preprocessing, feature engineering, regression algorithms, and real-world ML applications.

---

⭐ If you find this project interesting, feel free to explore the repository!
