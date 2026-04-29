
---

# 🌐 2. WEB PORTAL README.md

👉 Repo: `web-portal`

```md
# Web Portal - Gender Classification API Client

## 📌 Overview
This is a simple frontend web application that interacts with the backend API to display profile data.

It demonstrates integration between a frontend interface and a Django REST API backend.

---

## ⚙️ Tech Stack

- HTML
- CSS
- JavaScript (Fetch API)

---

## 🚀 Features

- Fetch profiles from backend API
- Display paginated results
- Basic UI for viewing data
- API integration using fetch()

---

## 🔐 Authentication

Requests include JWT token in headers:

headers: {
  "Authorization": "Bearer YOUR_ACCESS_TOKEN",
  "X-API-Version": "1"
}

Example API Call
fetch("https://gender-classification-api-production.up.railway.app/profiles", {
  method: "GET",
  headers: {
    "Authorization": "Bearer YOUR_ACCESS_TOKEN",
    "X-API-Version": "1"
  }
})
.then(res => res.json())
.then(data => console.log(data));

### 🧠 Limitations
1. No login UI (token must be manually added)
2. Minimal UI styling
3. No state management