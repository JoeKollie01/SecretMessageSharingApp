# 🔐 Secret Message Sharing App

This is a lightweight web app that lets users create and share secret messages via encrypted URLs. When someone opens the link, they can view the original message — but only once!

## 🚀 Live Demo

Try it here: [https://secret-message-sharing-app-tau-sand.vercel.app/](https://secret-message-sharing-app-tau-sand.vercel.app/)

## 📦 Features

- Enter a secret message and generate a unique URL.
- The message is **Base64 encoded** and embedded in the URL hash (`#`).
- When someone opens the link, the secret is revealed **only to them**, and the form is hidden.
- All logic runs client-side, with no server or database required.

## 💡 How It Works

1. User inputs a message and submits the form.
2. The message is encoded with `btoa()` and appended to the URL as a hash.
3. A new form appears with a link to share.
4. When someone visits that link, `app.js` decodes the message from the URL hash using `atob()` and displays it.

## 🧪 Tech Stack

- HTML
- CSS (with [Materialize CSS](https://materializecss.com/))
- Vanilla JavaScript

## 📁 Project Structure

📁 secret-message-app/ ├── index.html # Main webpage ├── style.css # Styling and layout └── app.js # JavaScript logic for encoding/decoding messages


## 🛠 How to Run Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/secret-message-sharing-app.git
   cd secret-message-sharing-app
