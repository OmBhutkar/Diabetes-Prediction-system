# Diabetes-Prediction-system

---

## Diabetes Prediction Web App

### Overview:
This project is a web application that predicts the likelihood of a person having diabetes based on a set of medical parameters, such as glucose level, blood pressure, BMI, and more. Built using **Flask** for the backend and **HTML/CSS/JavaScript** for the frontend, the app allows users to input their details, upload a photo, and receive a prediction about whether they have diabetes or not. Additionally, the app generates a **PDF report** summarizing the prediction and suggesting precautions and medications.

### Features:
- **User Input**: The application takes in various medical parameters like pregnancies, glucose, blood pressure, insulin levels, BMI, and age through an easy-to-use form.
- **Prediction Model**: A **Random Forest** classifier, trained on a diabetes dataset, predicts whether the user has diabetes based on the input data.
- **PDF Report Generation**: After prediction, a PDF report is generated, containing the user’s input data, prediction result, precautions, and suggested medications.
- **Downloadable Report**: The generated report can be downloaded via a direct link.
- **Photo Upload**: Users can upload a photo as part of the form submission (though not used for prediction purposes, the photo is displayed alongside the prediction result).
- **Responsive Design**: The frontend layout adjusts automatically for different screen sizes, with the uploaded photo displayed in the top-right corner for easy access.

### Tech Stack:
- **Backend**: 
  - **Flask**: A lightweight Python web framework to handle HTTP requests and run the machine learning model.
  - **scikit-learn**: Used for training the **Random Forest** classifier model.
- **Frontend**: 
  - **HTML/CSS**: Standard web technologies to structure and style the web pages.
  - **JavaScript**: Used for handling the form submission and dynamically displaying the prediction results.
  - **ReportLab**: Python library to generate the PDF report.
  
### Workflow:
1. **User Input**: The user enters their medical details into a form and uploads an optional photo.
2. **Prediction**: The form data is sent to the Flask backend, where the Random Forest model processes the data and generates a prediction (either "DIABETES" or "NO DIABETES").
3. **Results Display**: After the prediction, the result is displayed on the web page, along with precautions and medications based on the outcome.
4. **PDF Report**: A PDF report is generated that summarizes the user's inputs, the prediction, and suggestions. The report can be downloaded from the app.

### Installation:
To run this app locally, follow these steps:

1. **Clone the repository**:
   ```
   git clone https://github.com/your-username/diabetes-prediction-app.git
   cd diabetes-prediction-app
   ```

2. **Set up a virtual environment**:
   ```
   python -m venv venv
   source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
   ```

3. **Install dependencies**:
   ```
   pip install -r requirements.txt
   ```

4. **Run the app**:
   ```
   python app.py
   ```

5. **Access the app**: Open your web browser and go to `http://127.0.0.1:5000` to start using the app.

### Requirements:
- Python 3.x
- Flask
- scikit-learn
- pandas
- numpy
- reportlab

### Usage:
- On the homepage (`/`), fill out the form with your details and click "Predict".
- The result, including the prediction and a downloadable report, will appear below the form.
- You can download the PDF report containing the prediction results, precautionary advice, and suggested medications.

### Example Input:
- **Pregnancies**: 3
- **Glucose**: 120
- **Blood Pressure**: 70
- **Skin Thickness**: 25
- **Insulin**: 85
- **BMI**: 30.5
- **Diabetes Pedigree Function**: 0.5
- **Age**: 45

### Contributing:
Feel free to fork this repository and submit pull requests. Contributions, bug reports, and feature requests are always welcome!

### License:
This project is licensed under the MIT License.

---

