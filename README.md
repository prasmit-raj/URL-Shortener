# 🔗 URL Shortener

A scalable URL Shortener built with **Node.js**, **Express.js**, and **PostgreSQL/MongoDB**. This application converts long URLs into short, shareable links, redirects users to the original destination, and tracks basic analytics such as click counts.

This project is designed to strengthen backend development skills by implementing real-world concepts including REST APIs, database integration, routing, validation, and scalable application architecture.

---

## ✨ Features

* 🔗 Shorten long URLs into unique, shareable links
* 🚀 Redirect short URLs to their original destination
* 💾 Store URL mappings in a database
* 🎲 Generate unique short codes
* 📊 Track click counts for each shortened URL
* ✅ Input validation and error handling
* 🌐 RESTful API architecture
* ⚙️ Environment-based configuration using `.env`
* 📈 Designed with scalability in mind

---

## 🛠 Tech Stack

| Technology           | Usage                 |
| -------------------- | --------------------- |
| Node.js              | Runtime Environment   |
| Express.js           | Backend Framework     |
| PostgreSQL / MongoDB | Database              |
| dotenv               | Environment Variables |
| Git & GitHub         | Version Control       |

---

## 📂 Project Structure

```
url-shortener/
│
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   ├── services/
│   ├── utils/
│   └── app.js
│
├── config/
├── .env
├── package.json
└── README.md
```

---

## 🚀 Getting Started

### Clone the Repository

```bash
git clone https://github.com/your-username/url-shortener.git
cd url-shortener
```

### Install Dependencies

```bash
npm install
```

### Configure Environment Variables

Create a `.env` file in the project root.

Example:

```env
PORT=5000
DATABASE_URL=your_database_connection_string
BASE_URL=http://localhost:5000
```

### Run the Server

```bash
npm run dev
```

or

```bash
npm start
```

---

## 📌 API Endpoints

### Create Short URL

```
POST /api/shorten
```

Request Body

```json
{
  "url": "https://example.com/very/long/url"
}
```

Response

```json
{
  "shortUrl": "http://localhost:5000/abc123"
}
```

---

### Redirect

```
GET /:shortCode
```

Redirects the user to the original URL.

---

### Get URL Statistics

```
GET /api/stats/:shortCode
```

Returns:

* Original URL
* Short URL
* Total Clicks
* Creation Date

---

## 🎯 Learning Objectives

This project focuses on learning and implementing:

* REST API Design
* Backend Architecture
* Database Design
* URL Encoding
* Routing
* Middleware
* Input Validation
* Error Handling
* Environment Configuration
* Deployment Best Practices

---

## 🔮 Future Improvements

* User Authentication
* Custom Short URLs
* QR Code Generation
* Link Expiration
* Password-Protected Links
* Rate Limiting
* Redis Caching
* Docker Support
* Analytics Dashboard
* Swagger API Documentation
* Unit & Integration Testing
* CI/CD Pipeline

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## ⭐ Support

If you found this project helpful, consider giving it a **⭐ Star** on GitHub. It helps motivate continued development and improvements.
