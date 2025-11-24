# ❤️ Heart Disease Prediction Web App

This project is a **Streamlit-based web application** that predicts the
likelihood of **heart disease** using a trained machine learning model
(`model.pkl`).\
It also provides dataset visualization using **Seaborn** and **Plotly**.

------------------------------------------------------------------------

## 🚀 Features

### 1. **Home Page**

-   Overview of the application\
-   Displays an awareness image\
-   Explains the purpose of the tool

### 2. **Heart Disease Prediction**

Users provide the following inputs: - Age\
- Sex\
- Chest Pain Type (`cp`)\
- Resting Blood Pressure (`trestbps`)\
- Cholesterol Level (`chol`)\
- Fasting Blood Sugar (`fbs`)\
- Resting ECG Results (`restecg`)\
- Maximum Heart Rate (`thalach`)\
- Exercise-Induced Angina (`exang`)\
- Oldpeak Value (`oldpeak`)\
- Slope (`slope`)\
- Number of Major Vessels (`ca`)\
- Thalassemia (`thal`)

The machine learning model then outputs: - **Heart Disease Detected**
or\
- **No Heart Disease**

------------------------------------------------------------------------

## 📁 Project Structure

    ├── heart_disease_predict.py     # Streamlit app code
    ├── model.pkl                    # Trained ML model
    ├── Heart_Disease_Prediction.csv # Dataset used for training
    ├── .gitignore                   # used to ignore some files like virtual enviroment
    └── README.md                    # Documentation
  
   
------------------------------------------------------------------------

## 🧠 Machine Learning Model

-   The app loads a pre-trained model from `model.pkl`\
-   Inputs are converted into a NumPy array\
-   Passed into `model.predict()`\
-   Prediction:
    -   `1` → Heart Disease Detected\
    -   `0` → No Heart Disease

------------------------------------------------------------------------

## ▶️ How to Run the App

### Step 1: Install Dependencies

    pip install streamlit numpy pandas matplotlib seaborn plotly scikit-learn

### Step 2: Run Streamlit App

    streamlit run heart_disease_predict.py

The app will automatically open in your browser.

------------------------------------------------------------------------

## 📊 Visualizations

### **Non-Interactive Plot**

-   Uses Seaborn `lmplot`\
-   Shows correlation between:
    -   Cholesterol levels\
    -   Age\
    -   Split by sex\
    -   Colored by heart disease presence

### **Interactive Plot**

-   Uses Plotly 2D Hexbin\
-   Users can select:
    -   X-axis\
    -   Y-axis\
    -   Bin size

------------------------------------------------------------------------

## 📝 Requirements

-   Python 3.7+\
-   Streamlit\
-   Numpy\
-   Pandas\
-   Matplotlib\
-   Seaborn\
-   Plotly

------------------------------------------------------------------------

## 💡 Future Improvements

-   Deploy the app on Render/Streamlit Cloud\
-   Add feature importance graphs\
-   Show model accuracy reports\
-   Improve UI/UX

------------------------------------------------------------------------

## 🙌 Acknowledgements

-   Machine Learning Model: Scikit-learn\
-   Frontend: Streamlit\
-   Visualizations: Matplotlib, Seaborn, Plotly\
-   Dataset: Heart Disease Prediction Dataset
