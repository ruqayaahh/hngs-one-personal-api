# Simple Express API

A lightweight REST API built with Node.js and Express that exposes three endpoints. Deployed live on AWS EC2.

---

## 🚀 Live Deployment

**Base URL:** [https://aderinola.duckdns.org/](https://aderinola.duckdns.org/)

---

## 🛠️ Tech Stack

- **Runtime:** Node.js
- **Framework:** Express.js
- **Cloud Provider:** AWS
- **Web Server:** Nginx (Reverse Proxy)
- **SSL/TLS:** Let's Encrypt (Certbot)
- **Process Management:** PM2 (for persistence and auto-restarts)
- **Security:** UFW (Uncomplicated Firewall)

---

## 📦 Running Locally

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher recommended)

### Steps

1. **Clone the repository**

   ```bash
   git clone hhttps://github.com/ruqayaahh/hngs-one-personal-api.git
   cd hngs-one-personal-api
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start the server**

   ```bash
   npm start
   ```

   The server will start on **http://localhost:3000** by default.

   > For development with auto-restart on file changes:
   > ```bash
   > npm run dev
   > ```

---

## 📡 API Endpoints

All endpoints return `Content-Type: application/json`, HTTP status `200`, and respond within `500ms`.

---

### `GET /`

Returns a confirmation that the API is running.

**Request**
```
GET https://aderinola.duckdns.org/
```

**Response**
```json
{
  "message": "API is running"
}
```

---

### `GET /health`

Returns the health status of the API.

**Request**
```
GET https://aderinola.duckdns.org/health
```

**Response**
```json
{
  "message": "healthy"
}
```

---

### `GET /me`

Returns personal/profile information.

**Request**
```
GET https://aderinola.duckdns.org/me
```

**Response**
```json
{
  "name": "Ruqayaah Aderinola Sabitu",
  "email": "aderinolaruqayaah@gmail.com",
  "github": "https://github.com/ruqayaahh"
}
```

---

## 📁 Project Structure

```
.
├── index.js       # Main application entry point
├── package.json    # Project metadata and dependencies
└── README.md       # Project documentation
```

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).