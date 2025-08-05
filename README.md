# ☕ Crema di Caffè – Italian Café Web Application

**Crema di Caffè** is a fully functional, Italian-themed café website built from scratch. It features a beautiful frontend with an interactive menu and cart, supported by a Python Flask backend that handles menu data and cart operations. Designed for both elegance and usability, it mimics a real-world online ordering experience.

---

## 🌐 Live Pages (Frontend)
- **🏠 Home** – Welcome message, hero image, and call-to-action
- **📋 Menu** – Interactive category-based menu (Coffee, Tea, Snacks)
- **🛒 Cart** – Add-to-cart, quantity management, total pricing

---

## ⚙️ Backend (Flask API)
- 📦 Built in Python using Flask
- Serves menu data from `menu.json`
- Manages a session-free in-memory cart
- Checkout endpoint for clearing the cart

---

## 📁 Folder Structure

- `crema-di-caffe/`
  - `backend/`
    - `app.py` – Flask app entry point
    - `menu.json` – Static menu data
    - `requirements.txt` – Backend dependencies
    - `routes/`
      - `menu_routes.py` – Handles `/menu` API
      - `cart_routes.py` – Handles `/cart` API
    - `controllers/`
      - `menu_controller.py`
      - `cart_controller.py`
  - `frontend/`
    - `index.html` – Home page
    - `menu.html` – Menu page
    - `cart.html` – Cart page
    - `css/`
      - `style.css` – Frontend styling
    - `js/`
      - `script.js` – Cart & menu interactivity
  - `README.md` – Project documentation

---

## 🔌 API Endpoints

| Method | Endpoint         | Description                  |
|--------|------------------|------------------------------|
| GET    | `/menu`          | Fetch all menu items         |
| GET    | `/menu?category=coffee` | Filter items by category    |
| GET    | `/cart`          | View current cart contents   |
| POST   | `/cart/add`      | Add item to the cart         |
| POST   | `/cart/update`   | Update item quantity         |
| POST   | `/cart/checkout` | Checkout and clear the cart  |

---

## 🛠️ Tech Stack

### Frontend:
- HTML5, CSS3, JavaScript
- Optional: React.js + Tailwind CSS (if modern SPA)

### Backend:
- Python 3
- Flask
- Static JSON for menu items

---

## 🚀 Getting Started

### Backend
```bash
cd backend/
python3 -m venv venv
source venv/bin/activate  # or venv\Scripts\activate
pip install -r requirements.txt
python app.py
