# Cardiac Stroke Prediction System Using Machine Learning

## Overview

The **Cardiac Stroke Prediction System** is a web-based application designed to help predict the likelihood of a stroke in patients based on entered symptoms. The application provides a user-friendly dashboard where the user can input symptoms, and the system will process the data to generate a pie chart that predicts the chances of a stroke. 

This project is built using Machine Learning algorithms for the prediction model, and the front-end and back-end technologies are integrated to offer real-time prediction results.

## Features

- User-friendly dashboard for inputting patient symptoms.
- Real-time prediction of stroke risk displayed as a pie chart.
- Frontend developed using HTML, CSS, JavaScript, and Bootstrap.
- Backend powered by Python for the stroke prediction algorithm.
- MySQL database for data storage and management, initialized using XAMPP.
- Results displayed on the local web server via Apache, accessible on the browser (Chrome).

## Technologies Used

### Frontend:
- **HTML5**: For structuring the web pages.
- **CSS3**: For styling and layout.
- **JavaScript**: For interactive features and real-time data rendering.
- **Bootstrap**: For responsive design and pre-built UI components.

### Backend:
- **Python**: For building the prediction model using machine learning.
- **MySQL (XAMPP)**: For storing patient data and handling database operations.
- **XAMPP (Apache & MySQL)**: Used to initialize the local server for running the web app.

### Libraries and Tools:
- **Matplotlib**: For rendering pie charts based on prediction results.
- **Flask**: For creating a simple web framework to manage data flow between the frontend and backend.
- **Machine Learning Libraries**: Scikit-learn, Pandas, and NumPy for implementing the prediction model.

## How It Works

1. **Symptoms Input**:  
   The user enters patient symptoms into the dashboard (e.g., age, blood pressure, medical history).
   
2. **Data Processing**:  
   The system processes the input using a machine learning model (e.g., logistic regression or decision trees) to predict the risk of a stroke.

3. **Prediction Display**:  
   The result is displayed as a pie chart on the same dashboard. The pie chart shows the probability of whether the patient might experience a stroke or not.

## Setting Up the Project

### Requirements

- **XAMPP**: Install and configure XAMPP to run MySQL and Apache servers.
- **Python**: Ensure Python is installed along with the required libraries.
- **MySQL**: Use MySQL for the database, available through XAMPP.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/Cardiac-Stroke-Prediction-System.git
    ```

2. Install Python libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. Start XAMPP:
    - Run **Apache** and **MySQL** using XAMPP Control Panel.
    - Import the database SQL file into MySQL via PHPMyAdmin.

4. Configure MySQL connection:
    - Update the database connection settings in the Python backend file to match your MySQL configuration.

5. Run the application:
    ```bash
    python app.py
    ```

6. Open the browser and visit:
    ```bash
    http://localhost:5000
    ```

### File Structure

```plaintext
├── static/
│   ├── css/
│   ├── js/
│   ├── images/
├── templates/
│   ├── index.html
│   └── dashboard.html
├── app.py
├── model.py
├── requirements.txt
├── README.md
└── database.sql
```

- **static/**: Contains CSS, JavaScript, and images for the frontend.
- **templates/**: HTML files that render the UI for the dashboard and results.
- **app.py**: Main Python file to run the server and manage routes.
- **model.py**: Python file for the stroke prediction model.
- **requirements.txt**: Lists the dependencies for the project.
- **database.sql**: SQL file to set up the required database.

## Usage

1. Launch the app by running the `app.py` file and opening the browser at `localhost`.
2. Enter the symptoms of the patient on the dashboard.
3. Click on "Predict" to generate the stroke prediction.
4. The result will be displayed as a pie chart indicating the probability of stroke.

## Future Improvements

- Add more advanced machine learning models for better accuracy.
- Include more symptoms and risk factors for a more comprehensive prediction.
- Integrate real-time data for updating patient records.

## License

This project is licensed under the MIT License.
