# 📰 DjangoChronicle – Your Personal CRM!  

Welcome to **DjangoChronicle**, a **Customer Relationship Management (CRM) System** built with **Django** and **MySQL**! 🎉  

This project allows users to **register, log in, manage customer records**, and perform CRUD operations in a secure and organized way. Whether you're handling a small business or just love managing data, DjangoChronicle is here to help! 💼📊  

---

## 🚀 Features  

✔️ **User Authentication** (Login, Register, Logout) 🔑  
✔️ **View, Add, Update, and Delete** customer records 📝  
✔️ **Secure MySQL Database Integration** 🛢️  
✔️ **Bootstrap-Styled UI** for a clean look 🎨  
✔️ **Django Messages Framework** for real-time notifications 📢  

---

## 🛠 Tech Stack  

Here's what powers DjangoChronicle ⚡:  

🔹 **Backend:** Django (Python) 🐍  
🔹 **Database:** MySQL 🛢️  
🔹 **Frontend:** HTML, CSS, Bootstrap 🎨  
🔹 **Authentication:** Django’s built-in auth system 🔐  

---

## 🏗️ Installation Guide  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/yourusername/DjangoChronicle.git
cd DjangoChronicle
```

### 2️⃣ Install Dependencies  
```bash
pip install django
pip install mysql-connector-python
```

### 3️⃣ Set Up MySQL Database  
Make sure MySQL is installed and running. Get it from:  
🔗 [MySQL Installer](https://dev.mysql.com/downloads/installer/)  

Then, create a database using the provided script in **mydb.py** 📜:  
```python
import mysql.connector
dataBase = mysql.connector.connect(
    host='localhost',
    user='root',
    passwd='yourpassword'
)
cursorObject = dataBase.cursor()
cursorObject.execute("CREATE DATABASE djangochronicle")
```

### 4️⃣ Apply Migrations  
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5️⃣ Create a Superuser  
```bash
python manage.py createsuperuser
```

### 6️⃣ Run the Server 🚀  
```bash
python manage.py runserver
```
Now, open **http://127.0.0.1:8000/** in your browser! 🌍  

---

## 📂 Project Structure  

```
📦 DjangoChronicle
 ┣ 📂 website/ (Main Django App)
 ┃ ┣ 📜 views.py (Handles authentication & records)
 ┃ ┣ 📜 urls.py (Defines all routes)
 ┃ ┣ 📜 models.py (Defines database schema)
 ┃ ┣ 📜 forms.py (Handles user input forms)
 ┣ 📜 manage.py (Django project manager)
 ┣ 📜 mydb.py (Database setup script)
 ┗ 📜 README.md (You are here! 📖)
```

---

## 🎯 How to Use  

1️⃣ **Register/Login** to access the dashboard.  
2️⃣ **Manage customer records** (Add, Edit, Delete).  
3️⃣ **View detailed records** securely.  
4️⃣ **Logout** when done. (Don't forget! 😉)  

---

## 🚀 Future Improvements  

✅ Adding an **API** for external integrations.  
✅ Implementing **search and filters** for customer records.  
✅ Enhancing UI with **custom themes**.  

---

## 🤝 Open for Collaboration!  

Hey you! Yes, you! 👀 If you have ideas, suggestions, or want to make DjangoChronicle even better, feel free to:  

🔹 Open an **issue** or **pull request** on GitHub! 🛠️  
🔹 Share feedback and improvements! ✨  
🔹 Tell me if my code is a disaster and help fix it! 😂  

I’d be thrilled if you contribute! Let’s build something awesome together! 🚀🎉  
