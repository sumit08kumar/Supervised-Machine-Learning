
# 🌐 Language Translator App

This is a simple web application that translates text from one language to another using **IBM Watson Language Translator** API. The app is built using **Flask (Python)** and deployed on **Heroku**.

## 🔧 Tech Stack

* **Frontend**: HTML, CSS, Bootstrap
* **Backend**: Python, Flask
* **API**: IBM Watson Language Translator
* **Deployment**: Heroku

---

## 📦 Features

* Translate text between multiple languages
* Clean and simple UI
* Uses IBM Watson for high-quality translations
* Easy deployment on Heroku

---

## 🧠 Prerequisites

* IBM Cloud account
* Heroku account
* Python 3.x
* Git

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/language-translator-app.git
cd language-translator-app
```

### 2. Create a virtual environment and install dependencies

```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Get IBM Cloud Language Translator Credentials

1. Go to [IBM Cloud Console](https://cloud.ibm.com)
2. Create a **Language Translator** service
3. Get your **API Key** and **URL**
4. Create a `.env` file in the project root and add:

```env
API_KEY=your_ibm_api_key
API_URL=your_ibm_service_url
```

### 4. Run the app locally

```bash
flask run
```

---

## 🌍 Deployment on Heroku

### 1. Create `Procfile`

```Procfile
web: gunicorn app:app
```

### 2. Create `requirements.txt` and `runtime.txt`

```bash
pip freeze > requirements.txt
echo "python-3.11.4" > runtime.txt  # use your Python version
```

### 3. Commit to Git

```bash
git init
git add .
git commit -m "Initial commit"
```

### 4. Create Heroku App and Push

```bash
heroku login
heroku create translator-ibm-app
heroku config:set API_KEY=your_ibm_api_key
heroku config:set API_URL=your_ibm_service_url
git push heroku master
```

## 🧪 Sample Usage

* Enter text: `"Hello, how are you?"`
* Select language: `English to Spanish`
* Result: `"Hola, ¿cómo estás?"`

---

## 📄 License

This project is licensed under the MIT License.

