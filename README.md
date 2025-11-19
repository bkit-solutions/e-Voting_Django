# 🗳️ e-Voting System (Django)

<p align="center">
A secure, modern, OTP-based online voting system built using <b>Django</b>.  
Designed for colleges, organizations, and institutions requiring a reliable digital voting platform.
</p>

<p align="center">
<img src="https://cdn-icons-png.flaticon.com/512/1041/1041916.png" width="130">
</p>

---

## 📌 Overview
**e-Voting Django** is a secure and user-friendly digital voting system featuring OTP verification, voter authentication, admin-controlled elections, and automated result generation.

Built with **Django**, the system ensures security, transparency, and easy deployment.

---

## ⚡ Core Features

### 🧑‍💻 User Features
- Voter login with email OTP verification  
- Vote once per election (strict protection)  
- View candidate list  
- Cast vote securely  
- Receive confirmation  

### 🛂 Admin Features
- Create and manage elections  
- Add/update/delete candidates  
- Voter registration management  
- Real-time vote counting  
- View & publish final results  

### 🔐 Security
- OTP-based login  
- Unique vote enforcement  
- Secure session handling  
- 2-step email authentication for sending OTP  

---

## 🛠 Tech Stack

### **Backend**
- Python  
- Django  
- Django ORM  
- SQLite / PostgreSQL  

### **Frontend**
- HTML / CSS  
- Bootstrap  
- Django templates  

---

## 🧪 Installation Guide

Follow these steps to run the project locally:

---

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/<your-org>/e-Voting_Django.git
cd e-Voting_Django
```

---

### **2️⃣ Create & Activate Virtual Environment**
```bash
python -m venv venv

# Windows
venv\Scripts\activate

# macOS/Linux
source venv/bin/activate
```

---

### **3️⃣ Install Requirements**
```bash
pip install -r requirements.txt
```

---

### **4️⃣ Run Migrations**
```bash
python manage.py migrate
```

---

### **5️⃣ IMPORTANT Email Configuration**
To enable OTP-based authentication, update the email settings.

Open:

```
Elections/settings.py
```

Replace the dummy Gmail & app password with your actual credentials.

### ⚠️ **IMPORTANT NOTE**
You MUST enable **Google 2‑Step Verification** and create an **App Password**.

Then update:

```python
EMAIL_HOST_USER = "your-email@gmail.com"     # Replace with your Gmail
EMAIL_HOST_PASSWORD = "your-app-password"    # Replace with 16-character app password
```

Without this, OTP emails will NOT be sent.

---

### **6️⃣ Create Superuser**
```bash
python manage.py createsuperuser
```

---

### **7️⃣ Start Development Server**
```bash
python manage.py runserver
```

---

### **8️⃣ Access the Platform**

| Feature | URL |
|--------|-----|
| 🗳️ Voting Portal | http://127.0.0.1:8000/ |
| 🔐 Admin Dashboard | http://127.0.0.1:8000/admin/ |

---

## 👥 Project Maintainer

<h3 align="center">BKIT</h3>

<p align="center">
Building secure, scalable, and innovative digital platforms.
</p>
