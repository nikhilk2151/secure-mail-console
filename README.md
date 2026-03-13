# 📧 Secure Mail Console

A powerful **web-based email sending console** built with **Node.js, Express, and Nodemailer** that allows users to send bulk emails securely using Gmail SMTP.
This tool provides a simple interface for sending emails to multiple recipients with real-time status updates.

---

## 🚀 Features

* Send emails using **Gmail SMTP**
* **Bulk email sending**
* Real-time sending status using **Socket.IO**
* Simple and clean **web interface**
* Supports **HTML email content**
* Secure backend with **Node.js**
* Cross-origin support using **CORS**
* Easy deployment on **VPS / cloud servers**

---

## 🛠 Tech Stack

**Frontend**

* HTML
* CSS
* JavaScript

**Backend**

* Node.js
* Express.js
* Socket.IO
* Nodemailer

**Email Service**

* Gmail SMTP

---

## 📂 Project Structure

```
secure-mail-console/
│
├── public/            # Frontend files
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── server.js          # Main backend server
├── package.json       # Project dependencies
└── README.md
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/secure-mail-console.git
```

### 2️⃣ Open the Project

```bash
cd secure-mail-console
```

### 3️⃣ Install Dependencies

```bash
npm install
```

---

## ▶️ Run the Application

Start the server using:

```bash
node server.js
```

or

```bash
npm start
```

The server will start on:

```
http://localhost:3000
```

Open this URL in your browser.

---

## 📧 SMTP Configuration

Edit the SMTP configuration in **server.js**

Example configuration:

```javascript
const transporter = nodemailer.createTransport({
  service: "gmail",
  auth: {
    user: "your-email@gmail.com",
    pass: "your-app-password"
  }
});
```

⚠️ **Important:**
Use a **Gmail App Password**, not your normal Gmail password.

---

## 🌐 Deployment

You can deploy this project on:

* Render
* Railway
* VPS Server
* DigitalOcean
* AWS EC2

For production deployment:

```bash
npm install pm2 -g
pm2 start server.js
```

---

## 🔒 Security Notes

* Always use **App Passwords** for Gmail SMTP.
* Do not upload sensitive credentials to GitHub.
* Use **environment variables (.env)** for production.

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 👨‍💻 Author

**Nikhil Kumar**

If you like this project, consider giving it a ⭐ on GitHub!
