
# 🔐 Secure Encrypted Notebook

A **fully client-side, end-to-end encrypted notebook web application** that allows users to securely create accounts, write notes, draw freely on an infinite canvas, and export everything as a PDF — all without using any backend servers or third-party authentication services.

This project demonstrates **real-world cryptographic design**, secure client-side storage, and advanced frontend engineering.

---

## 🚀 Features

* 🔒 **End-to-End Encryption (E2EE)**

  * AES-256-GCM encryption
  * PBKDF2 password-based key derivation (100,000 iterations)
  * Zero-knowledge architecture (data never leaves the browser unencrypted)

* 👤 **Secure Authentication**

  * Local account creation & login
  * No Google, Facebook, or third-party authentication

* 📝 **Encrypted Notes**

  * Titles, content, and drawings are fully encrypted before storage

* 🎨 **Advanced Drawing System**

  * Works on **desktop, mobile, tablet & stylus**
  * Infinite canvas expansion (similar to Microsoft OneNote)
  * Smooth real-time drawing

* 📄 **True PDF Export**

  * One-click encrypted note → PDF download
  * Text + drawings embedded into a clean PDF layout

* 🌐 **Fully Static & Serverless**

  * Works entirely in the browser
  * Compatible with GitHub Pages

---

## 🔐 Security Architecture

This project follows **zero-knowledge encryption principles**:

1. The user's password is never stored.
2. A cryptographic key is derived using **PBKDF2 + SHA-256**.
3. All notes and drawings are encrypted using **AES-256-GCM**.
4. Only encrypted data is stored in `localStorage`.
5. Without the correct password, **data is cryptographically unrecoverable**.

### Crypto Stack

| Component      | Algorithm                |
| -------------- | ------------------------ |
| Key Derivation | PBKDF2 (100k iterations) |
| Encryption     | AES-256-GCM              |
| Randomness     | Web Crypto API CSPRNG    |

This ensures:

* Confidentiality
* Integrity
* Authentication
* Replay attack resistance

---

## 🏗 Architecture

* **Frontend:** HTML, CSS, JavaScript
* **Crypto Engine:** Web Crypto API
* **Storage:** Browser LocalStorage (encrypted blobs only)
* **PDF Export:** jsPDF
* **Hosting:** GitHub Pages

---

## ⚙ How To Run Locally

Simply open the file:

```bash
index.html
```

Or use Live Server:

```bash
npx serve .
```

---

## 🌍 Deploying to GitHub Pages

1. Push this repository to GitHub
2. Go to **Settings → Pages**
3. Set source branch to `main`
4. Save

Your secure notebook will be live at:

```
https://<username>.github.io/<repo-name>/
```

---

## 🛡 Security Disclaimer

This project is intended for **educational and demonstration purposes**.

While strong cryptography is used, this application does **not replace professional-grade secure note platforms** and should not be used for storing highly sensitive real-world secrets.

---

## 🎯 Learning Outcomes

This project demonstrates:

* Client-side cryptography implementation
* Secure key management
* Zero-knowledge data models
* Canvas rendering & infinite scrolling systems
* PDF generation
* Secure UX design

---

## 👨‍💻 Author

**Mohamed Al Lawati**
Cybersecurity & Computer Science Student
German University of Technology in Oman (GUtech)

GitHub: [https://github.com/Mohd5L](https://github.com/Mohd5L)
LinkedIn: [https://linkedin.com/in/mohamed-allawati-8b30911b2/](https://linkedin.com/in/mohamed-allawati-8b30911b2/)

