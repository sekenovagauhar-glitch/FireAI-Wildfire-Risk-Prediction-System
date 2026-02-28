🔥 FireAI — Wildfire Risk Prediction System
📌 Project Description

FireAI — жасанды интеллектке негізделген жүйе, ол спутниктік деректерді пайдаланып, Қазақстан аумағында орман және дала өрттерінің пайда болу ықтималдығын болжайды.

Жүйе тарихи өрт деректерін талдап, кеңістік-уақыттық заңдылықтарды үйренеді және болашақ кезеңдер үшін өрт тәуекелінің картасын құрады.

🧠 Solution Architecture
Satellite Fire Data (CSV)
            ↓
Data Preprocessing
            ↓
Spatial Grid Creation
            ↓
Feature Engineering
            ↓
Machine Learning Model (Random Forest)
            ↓
Probability Prediction
            ↓
Risk Analysis & Visualization (Heatmap)
Architecture Components
Component	Description
Data Layer	Satellite fire detection dataset
Processing Layer	Data cleaning & aggregation
ML Layer	Random Forest classification model
Prediction Layer	Fire probability estimation
Visualization Layer	Interactive risk map
⚙️ Technology Stack
Programming

Python 3.10+

Libraries

numpy — numerical computations

pandas — data processing

scikit-learn — machine learning

matplotlib — visualization

folium — interactive maps

Data Source

Satellite wildfire detection datasets (CSV format)

🤖 AI Algorithms and Models
Machine Learning Model

Random Forest Classifier

Model predicts:

𝑃
(
fire occurrence
)
P(fire occurrence)

for each geographic grid cell and month.

Why Random Forest?

Handles nonlinear dependencies

Robust to noisy satellite data

Works well with tabular geospatial data

Reduces overfitting via ensemble learning

Feature Engineering

The model uses:

Feature Type	Description
Spatial features	Latitude & longitude
Temporal features	Month cyclic encoding (sin/cos)
Historical memory	Previous fire occurrences
Moving averages	Fire activity trends

Examples:

fire_lag1 — fire last month

fire_lag3 — fire 3 months ago

fire_lag12 — fire last year

🚀 Installation
1. Clone repository
git clone https://github.com/username/fireai.git
cd fireai
2. Create environment
python -m venv venv

Activate:

Windows

venv\Scripts\activate

Linux / Mac

source venv/bin/activate
3. Install dependencies
pip install -r requirements.txt
▶️ How to Run

1️⃣ Place wildfire dataset:

data/fire_data.csv

2️⃣ Open notebook:

FireAI_forecast.ipynb

3️⃣ Run all cells sequentially.

📊 Output

The system generates:

Fire probability predictions

Monthly risk rankings

Kazakhstan wildfire heatmap

Model performance metrics

Example outputs:

Accuracy

Precision

Recall

F1-score

🗺 Visualization

Interactive map shows wildfire risk intensity:

🔴 High risk

🟠 Medium risk

🟢 Low risk

📈 Model Evaluation

Metrics used:

Accuracy

Precision

Recall

F1-score

The model is validated using time-based train/test split to simulate real forecasting conditions.

🔬 Scientific Interpretation

Fire probability depends on:

seasonal climate cycles

historical fire activity

geographic location patterns

The model captures spatio-temporal wildfire dynamics.

📁 Project Structure
fireai/
│
├── data/
│   └── fire_data.csv
│
├── FireAI_forecast.ipynb
├── requirements.txt
└── README.md
👨‍💻 Author

Ғарыш зерттеушілері
AI & Environmental Data Research

📄 License

MIT License# FireAI-Wildfire-Risk-Prediction-System

