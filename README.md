# 🍔 Food Delivery System

### OOP-Based Food Delivery Application using Python & Streamlit

A practical **Food Delivery Management System** built with **Python Object-Oriented Programming (OOP)** and an interactive **Streamlit** interface.

The project models a simplified real-world food delivery workflow — from customer creation and wallet management to order placement, delivery-partner assignment, OTP verification, and successful delivery.

---

## 🚀 Live Demo

### [🍔 Open Food Delivery App](https://food-delivery-4vvzuk2ndranttfmrdbyna.streamlit.app/)

> **Try the application directly in your browser. No local setup required.**

---

## 📌 Overview

This project demonstrates how **Object-Oriented Programming principles** can be applied to design a real-world application.

The system consists of different entities such as:

- 👤 Customer
- 🏪 Restaurant
- 🍽️ Menu Item
- 🛒 Order
- 🛵 Delivery Partner

Each entity is represented using Python classes, with methods responsible for specific actions and behaviours.

The Streamlit interface provides an interactive way to use these OOP classes through a web application.

---

## 🔄 Application Workflow

```text
👤 Create Customer
        ↓
💰 Add Wallet Balance
        ↓
🍽️ View Restaurant Menu
        ↓
🛒 Select Food Items
        ↓
📦 Place Order
        ↓
🛵 Create Delivery Partner
        ↓
✅ Accept Order
        ↓
🔐 Verify OTP
        ↓
🎉 Complete Delivery
```

---

## ✨ Key Features

### 👤 Customer Management

- Create customer profile
- Store name, phone number and address
- Add funds to wallet
- Display current wallet balance

### 🍽️ Restaurant & Menu

- Restaurant information
- Multiple food items
- Veg / Non-Veg classification
- Food item pricing
- Interactive menu display

### 🛒 Order Management

- Select multiple food items
- Create customer orders
- Automatically generate Order IDs
- Calculate order bill
- Calculate GST
- Add packaging charges
- Display estimated delivery time
- Track order status

### 🛵 Delivery Partner Management

- Create delivery partner profile
- Store phone number
- Select delivery vehicle
- Track partner availability
- Accept customer orders

### 🔐 OTP-Based Delivery Verification

- Generate an order OTP
- Verify OTP before delivery
- Prevent delivery when an incorrect OTP is entered
- Mark the order as delivered after successful verification

### 📊 Order Tracking

The application follows the delivery lifecycle:

```text
Placed → Accepted → Delivered
```

### 🌐 Interactive Streamlit UI

- Clean web interface
- Interactive forms
- Buttons and selection controls
- Session-state based workflow
- Real-time order information
- Delivery status display

---

## 🧠 OOP Concepts Demonstrated

The project focuses on practical implementation of core Object-Oriented Programming concepts.

| Concept | Implementation |
|---|---|
| **Classes & Objects** | `User`, `Customer`, `Restaurant`, `MenuItem`, `Order`, `DeliveryPartner` |
| **Inheritance** | `Customer` and `DeliveryPartner` inherit from `User` |
| **Abstraction** | Abstract methods defined in `User` |
| **Encapsulation** | Internal attributes such as wallet balance and order status |
| **Polymorphism** | Subclasses provide their own implementations of common methods |
| **Methods & Behaviour** | Wallet management, ordering, OTP verification and delivery |

---

## 🏗️ Project Architecture

```text
                    ┌──────────────────────┐
                    │      Streamlit UI    │
                    │       app.py         │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │   OOP Business Logic │
                    │  food_delivery.py   │
                    └──────────┬───────────┘
                               │
             ┌─────────────────┼─────────────────┐
             ▼                 ▼                 ▼
        👤 Customer       🏪 Restaurant      🛵 Delivery
             │                 │                 │
             └─────────────────┼─────────────────┘
                               ▼
                         🛒 Order
                               │
                               ▼
                         🔐 OTP Check
                               │
                               ▼
                       📦 Delivered
```

---

## 📂 Project Structure

```text
Food-Delivery/
│
├── app.py
├── food_delivery.py
├── streamlit_app.py
├── requirements.txt
├── Food_Delivery_System_Notebook_pynb.ipynb
└── README.md
```

### File Description

| File | Purpose |
|---|---|
| `food_delivery.py` | Contains the core OOP classes and application logic |
| `app.py` | Streamlit interface for interacting with the food delivery system |
| `streamlit_app.py` | Additional Streamlit implementation/reference |
| `requirements.txt` | Python dependencies |
| `Food_Delivery_System_Notebook_pynb.ipynb` | Jupyter Notebook used for project development |
| `README.md` | Project documentation |

---

## 🛠️ Tech Stack

### Programming Language
- 🐍 Python

### Framework
- 🎈 Streamlit

### Concepts
- Object-Oriented Programming
- Abstraction
- Encapsulation
- Inheritance
- Polymorphism
- Session State

### Development Tools
- Jupyter Notebook
- VS Code
- Git
- GitHub

---

## ⚙️ Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/RoshuNaik/Food-Delivery.git
```

### 2. Open the project directory

```bash
cd Food-Delivery
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit application

```bash
streamlit run app.py
```

The application will open in your default browser.

---

## 🧪 Example User Journey

### Step 1 — Create Customer

Enter:

```text
Name
Phone
Address
```

Create the customer profile.

### Step 2 — Add Wallet Balance

Add money to the customer's wallet.

### Step 3 — Browse Menu

View available food items, prices and food type.

### Step 4 — Place Order

Select one or more food items and place the order.

The bill includes:

```text
Subtotal
   +
GST
   +
Packaging Fee
   =
Total Bill
```

### Step 5 — Create Delivery Partner

Enter the partner's:

```text
Name
Phone
Vehicle
```

### Step 6 — Accept Order

The available delivery partner accepts the customer's order.

### Step 7 — Verify OTP

Enter the OTP associated with the order.

### Step 8 — Complete Delivery

After successful OTP verification, the order is marked as:

```text
🎉 Delivered
```

---

## 📚 Learning Outcomes

This project helped demonstrate how Python OOP concepts can be translated into a practical application.

### Key learning areas

- Designing classes for real-world entities
- Creating relationships between objects
- Implementing inheritance
- Using abstract base classes
- Applying encapsulation
- Implementing polymorphic behaviour
- Managing application state
- Building an interactive UI with Streamlit
- Connecting Python backend logic with a web interface
- Using GitHub for project version control and collaboration

---

## 🔮 Future Enhancements

The application can be extended with:

- 🔐 User authentication
- 💳 Online payment integration
- 🗄️ MySQL / database integration
- 🏪 Multiple restaurants
- 🔎 Food and restaurant search
- ⭐ Customer ratings and reviews
- 🛵 Real-time delivery tracking
- 📊 Admin dashboard
- 🧾 Invoice generation
- 📧 Order notifications
- 📱 Mobile-responsive interface
- 📦 Multiple concurrent orders

---

## 👨‍💻 Author

### Roshan Vishnu Jadhav

**BCA | Python | SQL | Data Analytics**

🔗 **GitHub:**  
[github.com/RoshuNaik](https://github.com/RoshuNaik)

---

## ⭐ Project Highlights

> **A practical implementation of Object-Oriented Programming concepts through a real-world food delivery workflow, enhanced with an interactive Streamlit interface.**

If you find this project useful, consider giving the repository a ⭐.

---

### 🍔 Built with

**Python 🐍 · OOP 💡 · Streamlit 🎈 · GitHub 🚀**
