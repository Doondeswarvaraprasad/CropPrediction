🌾 Crop Recommendation Web App
🚀 AI-Powered Smart Agriculture
This project predicts the best crop to cultivate based on soil nutrients (N, P, K) and environmental factors (temperature, humidity, pH, rainfall). It leverages Machine Learning to help farmers make data-driven decisions and improve productivity.

✅ Problem Statement
Agriculture is highly dependent on weather and soil conditions. Farmers often lack data-driven recommendations for selecting the most suitable crop. This project solves this issue by using ML models trained on weather-based crop data to predict the best crop for given conditions.

📊 Dataset Information
Dataset: Weather-based crop dataset with soil nutrients & environmental factors

Features:

N - Nitrogen

P - Phosphorus

K - Potassium

temperature - Temperature in °C

humidity - Relative humidity %

ph - Soil pH

rainfall - Rainfall in mm

Target: Crop Label (22 different crops)

🧠 Model Workflow
Data Preprocessing: Handling missing values, normalization

Model Selection: Used ensemble approach (XGBoost + LightGBM + Random Forest)

Training: Split dataset into training/testing

Evaluation: Accuracy & Classification Report

Saving Model: Exported as crop_model.pkl for deployment

🏆 Model Performance
Model	Accuracy
Random Forest	97%
XGBoost	98%
LightGBM	98%
Voting Classifier	99%

✅ Features
✔️ Predicts the most suitable crop based on environmental parameters
✔️ Shows crop name with corresponding image
✔️ Modern UI with custom background and logo
✔️ High accuracy using ensemble ML model
✔️ Render Deployment Ready

🛠 Tech Stack
ML: XGBoost, LightGBM, Random Forest

Backend: Flask

Frontend: HTML, CSS (custom UI with background image)

Deployment: Render

📂 Project Structure
csharp
Copy
Edit
CropPrediction/
│── app.py                 # Flask Web App
│── crop_model.py          # Model Training Script
│── crop_model.pkl         # Trained Model
│── requirements.txt       # Dependencies
│── Procfile               # For Render Deployment
│
├── templates/
│    ├── index.html        # Input Page
│    └── result.html       # Output Page
│
├── static/
│    ├── style.css         # Custom Styles
│    ├── mylogo.png        # App Logo
│    └── images/           # Crop Images (apple.jpg, mango.jpg, etc.)
│
└── README.md              # Documentation
⚡ How to Run Locally
bash
Copy
Edit
# Clone the repo
git clone https://github.com/YourUsername/CropPrediction.git
cd CropPrediction

# Install dependencies
pip install -r requirements.txt

# Run the Flask app
python app.py
Then open http://127.0.0.1:5000 in your browser.

🌐 Deployment on Render
Ensure you have requirements.txt and Procfile

Push code to GitHub

On Render:

Build Command: pip install -r requirements.txt

Start Command: gunicorn app:app

🖼️ Screenshots
(Add after deployment)

👨‍💻 Author
Tammina Doondeswarvaraprasad
🎓 B.Tech CSE, KL University
🔥 AI/ML Developer | Full Stack Enthusiast

⭐ Support
If you like this project, give it a ⭐ on GitHub!

✅ This version includes:

Your dataset & workflow description

Model performance details

Deployment instructions

