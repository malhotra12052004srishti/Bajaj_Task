# 💡 BFHL - Bajaj Finserv Health Labs Backend Task

This is a backend API built using **Node.js** and **Express.js** as part of the BFHL backend evaluation task. The API processes a POST request with an array of alphanumeric and special characters and returns a structured response as per the given rules.

---

## 🚀 Hosted API

🔗 **Live URL:** (https://bajaj-task-t016.onrender.com/bfhl)  
🛠️ **Method:** `POST`  
📮 **Route:** `/bfhl`  
📦 **Content-Type:** `application/json`

---

## 📌 Features

- Takes an input array of mixed values.
- Separates numbers into **even** and **odd** arrays.
- Extracts **alphabets**, converts them to **uppercase**.
- Identifies and returns **special characters**.
- Calculates the **sum of numeric values**.
- Generates a **reversed, alternating caps string** using all alphabets.
- Generates a **custom user ID** in format: `full_name_ddmmyyyy`
- Returns a well-structured response with `is_success` flag.

---

## 📄 Request Example

```json
{
  "data": ["a", "1", "334", "4", "R", "$"]
}
✅ Response Example
json
Copy code
{
    "is_success": true,
    "user_id": "srishti_malhotra_12052004",
    "email": "srishti2408.be22@chitkara.edu.in",
    "roll_number": "2210992408",
    "odd_numbers": [
        "1"
    ],
    "even_numbers": [
        "334",
        "4"
    ],
    "alphabets": [
        "A",
        "R"
    ],
    "special_characters": [
        "$"
    ],
    "sum": "339",
    "concat_string": "Ra"
}


🧠 Tech Stack
Node.js

Express.js

Hosted on Render

🛠 How to Run Locally
Clone the repo:

bash
Copy code
git clone https://github.com/yourusername/bfhl-api.git
cd bfhl-api
Install dependencies:

bash
Copy code
npm install
Start the server:

bash
Copy code
npm start
Test on http://localhost:3000/bfhl using Postman or cURL.

🧹 Clean Code & Best Practices
Modular structure and clear route separation.

.gitignore excludes node_modules.

Clear error handling and status responses.

Fully documented README.md.

🤝 Author
Name: Srishti Malhotra

Email: srishtiludhian@gmail.com

GitHub: @malhotra12052004srishti

🌐 Deployment Info
Deployed via Render
Build Command: npm install
Start Command: npm start
Port: process.env.PORT

Feel free to fork the repo, raise issues, or contribute improvements! :)
