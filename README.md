# project_file_server


---

````markdown
# 📁 FileCloud – Simple File Sharing Server

**FileCloud** is a lightweight web-based file manager and downloader built with Node.js and Express. It allows users on the same network to browse, navigate, and download files via a clean user interface.

🔗 GitHub Repository: [https://github.com/sangrechy/project_file_server](https://github.com/sangrechy/project_file_server)

---

## 📦 Features

- 🗂️ Browse and navigate server folders
- 📥 Download files from the browser
- 🧭 Breadcrumb navigation
- 🎨 Dark mode modern UI
- 🛡️ Secured file path resolution
- 🚀 Ready for LAN usage (Wi-Fi or Ethernet)

---

## 📋 Requirements

- ✅ [Node.js](https://nodejs.org/) (LTS version recommended)
- No other tools or global installs required

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/sangrechy/project_file_server.git
cd project_file_server/app
````

### 2️⃣ Install Dependencies

```bash
npm install express multer
```

> Note: `path`, `fs`, and `os` are built-in Node.js modules—no installation required.

---

## 📁 Folder Structure

```txt
project_file_server/
│
├── /app
│   ├── app.js               # Express.js backend
│   ├── /public              # Static frontend assets
│   │   ├── index.html       # Main web interface
│   │   ├── script.js        # File/folder navigation logic
│   │   └── styles.css       # UI styling
│   ├── /files               # (Create manually) Shared files directory
│
├── README.md
├── LICENSE
```

> 🔧 Make sure to **create the `/files` folder** inside `/app/` to store files you want to share:

```bash
mkdir files
```

---

## ▶️ Run the Server

```bash
node app.js
```

You will see output like:

```txt
File manager running at http://192.168.1.5:3000
```

> Open that address in any device browser connected to the **same Wi-Fi network**.

---

## 🌐 Optional: External Access with Ngrok

To access from outside your local network:

1. Install [Ngrok](https://ngrok.com/)
2. Run:

```bash
ngrok http 3000
```

3. Share the public link Ngrok gives you (e.g. `https://abcd-1234.ngrok.io`)

---

## 🔐 Security Notes

* Access is strictly limited to files inside the `/files` directory
* No file uploads, deletions, or writes (read-only server)
* For uploading support, implement `multer` with proper route control

---

## 📜 License

This project is licensed under the **MIT License**

---

> 💡 Ideal for quick file sharing across mobile, laptop, or any device on your LAN

```

---


```
