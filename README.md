
# User Authentication System 🔐

A secure and scalable **User Authentication System** built using **Firebase Authentication**, **Google App Engine**, and **Cloud Firestore**. This project demonstrates how to manage user identity in a cloud-native, serverless environment with Python (Flask).

---

## 🚀 Features

* 🔑 **Firebase Authentication** – Secure login & credential management.
* ☁️ **Google App Engine** – Serverless deployment of the backend.
* 📂 **Cloud Firestore** – (Optional) user data & activity logging.
* ⚡ **Lightweight Flask API** – Verifies Firebase-issued ID tokens.
* 🔒 **Scalable & Secure** – Token-based authentication with minimal infra overhead.

---

## 🛠️ Tech Stack

* **Backend**: Python, Flask, Gunicorn
* **Authentication**: Firebase Authentication, Firebase Admin SDK
* **Database**: Cloud Firestore (Native Mode)
* **Cloud Hosting**: Google App Engine
* **Tools**: Google Cloud Console, gcloud CLI

---

## 🏗️ System Architecture

1. User signs in using Firebase Authentication.
2. Firebase generates a secure ID token.
3. Token is sent to Flask API (hosted on App Engine).
4. API validates token via Firebase Admin SDK.
5. (Optional) User details are stored in Firestore.
6. Response sent back to client (success/error).

---

## 📂 Project Structure

```
├── main.py             # Flask backend app  
├── firebase_config.json # Firebase service account key  
├── requirements.txt    # Python dependencies  
├── app.yaml            # App Engine deployment config  
└── README.md           # Project documentation
```

---

## ⚙️ Setup & Deployment

### 1️⃣ Prerequisites

* Google Cloud account with billing enabled
* Firebase project (Authentication & Firestore enabled)
* Python 3.9+

### 2️⃣ Clone the repo

```bash
git clone https://github.com/your-username/user-authentication-system.git
cd user-authentication-system
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Configure Firebase

* Download **firebase\_config.json** from Firebase Console
* Place it in the project root

### 5️⃣ Run locally

```bash
python main.py
```

Visit: `http://127.0.0.1:5000/`

### 6️⃣ Deploy on App Engine

```bash
gcloud app deploy
gcloud app browse
```

---

## 📸 Screenshots

*(Add your screenshots here – e.g., Firebase console, API responses, Firestore logs)*

---

## 🐛 Challenges Faced

* Billing setup issues on Google Cloud
* Flask & Werkzeug version conflicts
* IAM permissions for App Engine & Firestore

---

## ✅ Results

* Successfully deployed Flask API on Google App Engine
* Verified Firebase ID tokens securely
* Demonstrated optional Firestore logging

---

## 🔮 Future Enhancements

* Add frontend UI (HTML/React) for sign-up & login
* Support user role-based access
* Store login analytics in Firestore
* Integrate with GCP services like Pub/Sub & Cloud Functions

---

## 📜 License

This project is open-source and available under the **MIT License**.

---


