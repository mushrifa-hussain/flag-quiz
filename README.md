# 🏳️ Flag Quiz

A fun web quiz where users identify the **country based on its flag**.

Built using **Node.js, Express, PostgreSQL, and EJS**, this project shows a random flag and the user must guess the correct country name.
If the answer is correct ✅ the score increases.
If the answer is wrong ❌ the game ends.

---

## ✨ Features

🏳️ Random flag questions

🧠 Test knowledge of world flags

📊 Live score tracking

✔ Instant answer feedback

❌ Game ends on wrong answer

⚡ Fast Express server

🗄 Data stored in PostgreSQL

---

## 📸 Screenshots

(Add your screenshots here)

![Flag Quiz Screenshot](screenshots/app.png)

---

## 🛠 Tech Stack

**Backend**

* Node.js
* Express.js

**Frontend**

* EJS
* HTML
* CSS

**Database**

* PostgreSQL

---

## 📁 Project Structure

```
flag-quiz
│
├── public
│
├── views
│   └── index.ejs
│
├── flags.csv
├── index.js
├── package.json
└── package-lock.json
```

---

## 🗄 Database Setup

Create database

```
CREATE DATABASE world;
```

Create table

```
CREATE TABLE flags (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  flag VARCHAR(10)
);
```

Import the data from **flags.csv** into the table.

---

## ⚙ Database Configuration

Update the database credentials inside **index.js**.

```
const db = new pg.Client({
  user: "username",
  host: "localhost",
  database: "world",
  password: "password",
  port: port_number
});
```

Example:

```
const db = new pg.Client({
  user: "postgres",
  host: "localhost",
  database: "world",
  password: "your_password",
  port: 5432
});
```

---

## 💻 Installation

Clone the repository

```
git clone https://github.com/yourusername/flag-quiz.git
```

Go to the project folder

```
cd flag-quiz
```

Install dependencies

```
npm install
```

---

## ▶ Run the Application

```
node index.js
```

Open in your browser

```
http://localhost:3000
```

---

## 🎮 How the Quiz Works

1️⃣ The server loads country names and flags from PostgreSQL.

2️⃣ A random flag is selected.

3️⃣ The user enters the country name.

4️⃣ Correct answer → score increases 📈

5️⃣ Wrong answer → game over ❌

---

## 🚀 Future Improvements

⏳ Add timer for questions

🏆 Add leaderboard

🌎 Show capital city after correct answer

📊 Store high scores

🎯 Add difficulty levels

---

✨ *A fun way to learn world flags!* 🌍
