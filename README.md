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

<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/23c93d4f-deb7-455d-89bf-8f3475a97f63" />
<img width="1919" height="1028" alt="image" src="https://github.com/user-attachments/assets/b1d1cba2-5640-4d65-a603-22dce5e18e18" />

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
## ⚠️ Note

Flag emojis are rendered using **regional indicator symbols**.

On some systems (especially **Chrome on Windows**), the flags may appear as text like:

US
IN
FR

instead of flag emojis.

To properly view the flags, run the project in:

🦊 **Firefox browser**

This ensures the flags display correctly.

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
