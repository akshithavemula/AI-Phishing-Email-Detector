# AI-Phishing-Email-Detector
# 🛡️ AI Phishing Email Detector

An AI-powered web application that analyzes email content and classifies it as **Phishing/Suspicious** or **Legitimate** using Machine Learning.

The project uses **TF-IDF** for text feature extraction and a **Multinomial Naive Bayes** classifier for email classification. A **Flask** web application provides a simple interface for users to enter and analyze email content.

---

## 🚀 Features

* 📧 Analyze email content
* 🛡️ Detect potentially phishing or suspicious emails
* ✅ Identify legitimate emails
* 🤖 Machine Learning-based classification
* 📊 Display prediction confidence
* 🌐 Simple Flask web interface
* ⚡ Lightweight and beginner-friendly
* 🔐 Designed for cybersecurity learning and awareness

---

## 🧠 How It Works

The application follows this workflow:

```text
Email Content
     ↓
Text Preprocessing
     ↓
TF-IDF Feature Extraction
     ↓
Multinomial Naive Bayes
     ↓
Prediction
     ↓
Phishing / Legitimate
```

### 1. Email Input

The user pastes an email message into the web interface.

### 2. Feature Extraction

The text is converted into numerical features using **TF-IDF (Term Frequency-Inverse Document Frequency)**.

### 3. Machine Learning

A **Multinomial Naive Bayes** model analyzes the extracted features.

### 4. Classification

The model classifies the email as:

* ⚠️ Phishing / Suspicious
* ✅ Legitimate

### 5. Confidence

The application displays the model's estimated confidence for the prediction.

---

## 🛠️ Technologies Used

| Technology              | Purpose                   |
| ----------------------- | ------------------------- |
| Python                  | Programming language      |
| Flask                   | Web application framework |
| Pandas                  | Dataset processing        |
| NumPy                   | Numerical operations      |
| Scikit-learn            | Machine Learning          |
| TF-IDF                  | Text feature extraction   |
| Multinomial Naive Bayes | Email classification      |
| HTML                    | Web interface             |
| CSS                     | User interface styling    |
| Git & GitHub            | Version control           |

---

## 📁 Project Structure

```text
AI_phishing_detector/
│
├── app.py
├── train_model.py
├── dataset.csv
├── model.pkl
├── requirements.txt
├── README.md
├── .gitignore
│
├── templates/
│   └── index.html
│
└── static/
    └── style.css
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/AI-Phishing-Email-Detector.git
```

Go into the project directory:

```bash
cd AI-Phishing-Email-Detector
```

---

### 2. Create a virtual environment

```bash
python3 -m venv venv
```

Activate it:

### Linux / Kali Linux

```bash
source venv/bin/activate
```

### Windows

```powershell
venv\Scripts\activate
```

---

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🧪 Train the Machine Learning Model

Run:

```bash
python3 train_model.py
```

This trains the model using the dataset and generates:

```text
model.pkl
```

---

## ▶️ Run the Application

Start the Flask application:

```bash
python3 app.py
```

You should see something similar to:

```text
Running on http://127.0.0.1:5000
```

Open your browser and visit:

```text
http://127.0.0.1:5000
```

---

## 📧 Example

### Phishing Email

```text
URGENT! Your bank account has been suspended.
Click the link below immediately to verify your account.
Failure to verify your account within 24 hours will result in permanent suspension.
```

Expected classification:

```text
⚠️ Phishing / Suspicious Email
```

### Legitimate Email

```text
Hello,

The project meeting has been scheduled for tomorrow at 10 AM.
Please bring the latest project report.

Thank you.
```

Expected classification:

```text
✅ Legitimate Email
```

---

## 🔍 Machine Learning Model

The project uses a pipeline consisting of:

```text
TfidfVectorizer
       ↓
MultinomialNB
```

### TF-IDF

TF-IDF converts email text into numerical values based on the importance of words within the dataset.

### Multinomial Naive Bayes

Multinomial Naive Bayes is a commonly used classification algorithm for text-based problems such as spam and phishing email detection.

---

## 🔐 Cybersecurity Relevance

Phishing is a common social-engineering technique used to trick users into revealing sensitive information or interacting with malicious content.

This project demonstrates how Machine Learning can be applied to **email security and threat detection** by analyzing textual patterns.

It is intended for:

* Cybersecurity learning
* Machine Learning practice
* Phishing awareness
* Security research demonstrations
* Academic projects

---

## ⚠️ Limitations

This is an educational Machine Learning project and should not be considered a production-grade email security solution.

The model's predictions depend heavily on the quality and size of the training dataset.

A real-world phishing detection system could additionally analyze:

* Email headers
* Sender reputation
* URLs
* Domain age
* SPF/DKIM/DMARC results
* Attachments
* HTML content
* Redirect chains
* Threat intelligence
* Behavioral indicators

---

## 🔮 Future Improvements

Possible future enhancements include:

* 🔗 URL analysis
* 🌐 Malicious domain detection
* 📩 Email header analysis
* 🧠 Transformer-based NLP models
* 🤖 LLM-based phishing analysis
* 📊 Advanced risk scoring
* 🔍 Explainable AI
* 📈 Security analytics dashboard
* 🗃️ Larger real-world datasets
* 🔄 Continuous model retraining

---

## 👩‍💻 Author

**Akshitha Vemula**

Cybersecurity Enthusiast | AI & Cybersecurity Learner

Interested in:

* Cybersecurity
* Ethical Hacking
* Penetration Testing
* SOC & Threat Detection
* Artificial Intelligence
* Machine Learning

---

## 📜 Disclaimer

This project is created for **educational, research, and cybersecurity awareness purposes**.

The detection results should not be treated as a definitive security verdict. Users should independently verify suspicious emails and avoid opening unknown links or attachments.

---

## ⭐ Support

If you find this project useful for learning, consider giving the repository a ⭐ on GitHub.
