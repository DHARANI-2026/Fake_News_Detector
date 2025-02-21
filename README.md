📰 Fake News Detection Using Flask and Machine Learning
This project implements a web-based Fake News Detection system using Flask, a trained machine learning model, and a TF-IDF vectorizer. Users can enter news content, and the system predicts whether the news is REAL or FAKE.

🚀 Project Overview
Data Preparation: Dataset loaded from data/news.csv with title, text, and label columns.
Model Training: Random Forest Classifier trained on TF-IDF features.
Model Saving: Trained model and vectorizer saved as model.pkl and vectorizer.pkl in the models folder.
Flask Web App: User-friendly interface to check the authenticity of news articles.
📦 Project Structure
graphql
Copy
Edit
📁 Fake-News-Detection/
├── 📁 data/                # Dataset folder
│   └── news.csv            # Dataset with title, text, and label columns
├── 📁 models/              # Model folder
│   ├── model.pkl           # Trained Random Forest model
│   └── vectorizer.pkl      # TF-IDF vectorizer
├── 📁 templates/           # HTML templates for Flask
│   └── index.html          # User interface for input and results
├── app.py                  # Flask application for web interface
├── train_model.py          # Model training script
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation (this file)
⚙️ Installation & Setup
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/fake-news-detection.git
cd fake-news-detection
2. Create Virtual Environment (Optional but Recommended)
bash
Copy
Edit
# Windows
python -m venv venv
venv\Scripts\activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate
3. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
Generate requirements.txt:

bash
Copy
Edit
pip freeze > requirements.txt
📊 Dataset Structure (news.csv)
title	text	label
Example Title 1	Example text content	REAL
Example Title 2	Example text content	FAKE
🛠️ Model Training
To train the model, run:

bash
Copy
Edit
python train_model.py
Output:
models/model.pkl → Trained Random Forest model
models/vectorizer.pkl → TF-IDF vectorizer
🌐 Running the Flask App
Start the Flask web app:

bash
Copy
Edit
python app.py
Open http://127.0.0.1:5000/ in your browser.
🖼️ Example Output
Input: "COVID-19 vaccine found to have 95% effectiveness."
Prediction: ✅ The news is REAL.
📜 Key Features
User Input: Enter news content via a web form.
Prediction: Display "REAL" or "FAKE" based on the trained model.
Visualization: Accuracy and confusion matrix during training.
🤝 Contribution
Contributions are welcome!

Fork the project.
Create a branch (git checkout -b feature/new-feature).
Commit changes (git commit -m "Add new feature").
Push to branch (git push origin feature/new-feature).
Open a pull request.
