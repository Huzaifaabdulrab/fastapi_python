# FastAPI Side Hustles & Money Quotes API

This is a simple FastAPI project that provides a random **side hustle idea** or **money-related quote** when requested through API endpoints.

## Features
- Get a random **side hustle** idea.
- Get a random **money-related** quote.
- API key authentication for security.
- Built using **FastAPI** and Python.

---

## Installation & Setup

### 1️⃣ Clone the Repository
```sh
# Navigate to your desired directory
cd path/to/your/directory

# Clone this repository
git clone https://github.com/your-username/fastapi-side-hustles.git

# Move into the project folder
cd fastapi-side-hustles
```

### 2️⃣ Create a Virtual Environment
```sh
python -m venv .venv

# Activate the virtual environment (depending on OS)
# For Windows (CMD)
.venv\Scripts\activate
# For Windows (PowerShell)
.venv\Scripts\Activate.ps1
# For macOS/Linux
source .venv/bin/activate
```

### 3️⃣ Install Dependencies
```sh
pip install fastapi[standard] uvicorn
```

---

## Running the API Server

To start the FastAPI server, run:
```sh
uvicorn main:app --reload
```

Once the server is running, open **http://127.0.0.1:8000/docs** in your browser to explore the API using FastAPI’s built-in Swagger UI.

---

## API Endpoints

### 1️⃣ Get a Random Side Hustle Idea
**Endpoint:** `GET /side_hustles`

**Parameters:**
- `apiKey` (query parameter) → Required API key (`12345`)

**Example Request:**
```sh
GET http://127.0.0.1:8000/side_hustles?apiKey=12345
```

**Example Response:**
```json
{
  "side_hustle": "Freelancing - Start offering your skills online!"
}
```

---

### 2️⃣ Get a Random Money Quote
**Endpoint:** `GET /money_quotes`

**Parameters:**
- `apikey` (query parameter) → Required API key (`12345`)

**Example Request:**
```sh
GET http://127.0.0.1:8000/money_quotes?apikey=12345
```

**Example Response:**
```json
{
  "money_quote": "Money grows on the tree of persistence. – Japanese Proverb"
}
```

---

## Fixing Common Issues

### 1️⃣ Virtual Environment Activation Issue
If `.venv\Scripts\activate` is not found, create a new virtual environment:
```sh
python -m venv .venv
```
Then activate it and install dependencies again.


### 3️⃣ `fastapi[standard]` Installation Error
If you get an error about FastAPI dependencies, try installing using:
```sh
uv add fastapi[standard]
```

---

## License
This project is **open-source** and available for use under the MIT License.

---

### 🚀 Happy Coding with FastAPI! 🎉

