# 📧 Email Spam Classification

A full-stack machine learning application that detects spam emails using logistic regression. Built with Flask (backend) and Next.js (frontend).

## 🚀 Features

- **Real-time Spam Detection**: Paste email text and instantly classify it as spam or not spam
- **Machine Learning Powered**: Uses logistic regression with feature extraction
- **Modern UI**: Built with Next.js and Tailwind CSS
- **RESTful API**: Flask backend with CORS support
- **Trained Model**: Pre-trained model using SMS/email spam dataset

## 🛠️ Tech Stack

### Frontend
- **Next.js** - React framework for production
- **Tailwind CSS** - Utility-first CSS framework
- **React** - UI component library

### Backend
- **Flask** - Python web framework
- **Flask-CORS** - Cross-origin resource sharing
- **scikit-learn** - Machine learning library
- **pickle** - Model serialization

## 📋 Prerequisites

- Node.js (v14 or higher)
- Python (v3.8 or higher)
- pip (Python package manager)
- npm or yarn

## 🔧 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/email-spam-classification.git
cd email-spam-classification
```

### 2. Backend Setup

Navigate to the backend directory:
```bash
cd Back-End
```

Install Python dependencies:
```bash
pip install -r requirements.txt
```

Required packages:
```
flask
flask-cors
scikit-learn
pandas
numpy
pickle-mixin
```

### 3. Frontend Setup

Navigate to the frontend directory:
```bash
cd Email-Spam-Frontend/frontend
```

Install Node dependencies:
```bash
npm install
# or
yarn install
```

## 🚀 Running the Application

### Start the Backend (Flask API)

From the `Back-End` directory:
```bash
python app.py
```

The API will run on `http://localhost:5000`

### Start the Frontend (Next.js)

From the `Email-Spam-Frontend/frontend` directory:
```bash
npm run dev
# or
yarn dev
```

The application will run on `http://localhost:3000`

## 📡 API Endpoints

### `GET /`
Returns a welcome message confirming the API is running.

**Response:**
```json
"Spam Detection API is Running!"
```

### `POST /predict`
Classifies the provided email text as spam or not spam.

**Request Body:**
```json
{
  "mail": "Your email text here"
}
```

**Response:**
```json
{
  "prediction": "spam",
  "confidence": 0.95
}
```

**Error Response:**
```json
{
  "error": "No input provided"
}
```

## 📊 Model Information

- **Algorithm**: Logistic Regression
- **Feature Extraction**: Custom feature extraction pipeline
- **Training Data**: SMS Spam Collection Dataset
- **Model Files**:
  - `logistic_regression.pkl` - Trained model
  - `feature_extraction.pkl` - Feature vectorizer

## 📁 Project Structure

```
email-spam-classification/
├── Back-End/
│   ├── email_classification/
│   │   ├── logistic_regression.pkl
│   │   └── feature_extraction.pkl
│   ├── Model & Data set/
│   │   ├── sms spam classifier.ipynb
│   │   └── spam.csv
│   ├── app.py
│   ├── feature_extraction.pkl
│   ├── logistic_regression.pkl
│   └── requirements.txt
│
└── Email-Spam-Frontend/
    └── frontend/
        ├── .next/
        ├── dist/
        ├── node_modules/
        ├── public/
        ├── src/
        ├── .gitignore
        ├── jsconfig.json
        ├── next.config.mjs
        ├── package.json
        ├── postcss.config.mjs
        └── README.md
```

## 🧪 Usage Example

1. Start both backend and frontend servers
2. Open `http://localhost:3000` in your browser
3. Paste an email text in the input field
4. Click "Classify" or "Detect Spam"
5. View the result (Spam/Not Spam)

### Example Texts to Test

**Spam Example:**
```
URGENT! You have won $1,000,000! Click here to claim your prize now! 
Limited time offer. Reply with your bank details.
```

**Not Spam Example:**
```
Hi John, just wanted to confirm our meeting tomorrow at 3 PM. 
Let me know if you need to reschedule. Thanks!
```

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 👥 Authors

- Lakki ali  - [GitHub](https://github.com/yourusername)

## 🙏 Acknowledgments

- SMS Spam Collection Dataset
- scikit-learn documentation
- Flask and Next.js communities

## 📞 Contact
For questions or feedback, please open an issue or contact luckta.developer@gmail.com


⭐ Star this repository if you find it helpful!
