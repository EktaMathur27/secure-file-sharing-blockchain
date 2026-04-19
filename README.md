# secure-file-sharing-blockchain
# 🔐 Secure File Sharing System using Blockchain & IPFS

A full-stack application that enables **secure, decentralized, and tamper-proof file sharing** using encryption, IPFS, and blockchain technology.

---

## 🚀 Features

* 🔐 End-to-end file encryption
* 📦 Decentralized storage using IPFS
* ⛓️ Blockchain-based file integrity (Ethereum)
* 🔑 Secure download using unique key
* 📁 User dashboard with file management
* 🔍 Search functionality
* 📄 File preview (PDF/Image)
* 📊 Upload progress tracking
* 🎨 Modern UI with theme switch

---

## 🛠️ Tech Stack

* **Frontend:** React.js, Axios, CSS
* **Backend:** Flask (Python), Flask-CORS, JWT
* **Blockchain:** Solidity, Hardhat, Ethereum
* **Storage:** IPFS
* **Encryption:** Cryptography

---

## 📂 Project Structure

```
secure-file-sharing-blockchain/
│
├── backend/
│   ├── app.py
│   ├── encryption.py
│   ├── ipfs.py
│   ├── blockchain.py
│
├── blockchain/
│   ├── contracts/
│   ├── scripts/
│   ├── hardhat.config.js
│
├── frontend/
│   ├── src/
│   ├── App.js
│
└── README.md
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/secure-file-sharing-blockchain.git
cd secure-file-sharing-blockchain
```

---

### 2️⃣ Backend Setup

```bash
cd backend
python -m venv venv
venv\Scripts\activate   # Windows
pip install -r requirements.txt
python app.py
```

Backend runs on:

```
http://127.0.0.1:5000
```

---

### 3️⃣ Blockchain Setup

```bash
cd blockchain
npm install
npx hardhat node
npx hardhat run scripts/deploy.js --network localhost
```

---

### 4️⃣ IPFS Setup

Run IPFS daemon:

```bash
ipfs daemon
```

---

### 5️⃣ Frontend Setup

```bash
cd frontend
npm install
npm start
```

Frontend runs on:

```
http://localhost:3000
```

---

## 🔑 API Endpoints

| Method | Endpoint                     | Description           |
| ------ | ---------------------------- | --------------------- |
| POST   | `/login`                     | User login            |
| POST   | `/upload`                    | Upload encrypted file |
| GET    | `/download/<hash>?key=<key>` | Download file         |
| GET    | `/myfiles`                   | Get user files        |

---

## 🔐 How It Works

1. User logs in using JWT authentication
2. File is encrypted before upload
3. Encrypted file is stored on IPFS
4. IPFS hash is stored on blockchain
5. File can be securely downloaded using hash + key

---

## 📸 Screenshots

> Add your dashboard screenshots here

---

## 👨‍💻 Author

**Himanshu Rathore** 🚀

---

## ⭐ Future Improvements

* MongoDB integration (persistent storage)
* Cloud IPFS (Infura/Pinata)
* MetaMask wallet authentication
* File sharing via links

---

## 📜 License

This project is for educational and portfolio purposes.
