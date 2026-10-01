# Food-Delivery
Food Delivery System using Python and Streamlit

# 🍔 Food Delivery System — OOP Python + Streamlit

A simple and interactive **Food Delivery Management System** built using **Object-Oriented Programming (OOP) in Python** with a **Streamlit web interface**.

The project demonstrates how real-world food delivery workflows can be modelled using classes, objects, inheritance, abstraction, encapsulation, and method-based interactions.

## 🚀 Live Demo

👉 **https://food-delivery-4vvzuk2ndranttfmrdbyna.streamlit.app/**

Try the application directly in your browser without installing anything.

---

## 📌 Project Overview

This project simulates a basic food delivery workflow starting from customer creation and wallet management to placing an order, assigning a delivery partner, verifying an OTP, and completing the delivery.

### 🔄 Complete Workflow

```text
Create Customer
      ↓
Add Wallet Balance
      ↓
View Restaurant Menu
      ↓
Select Food Items
      ↓
Place Order
      ↓
Create Delivery Partner
      ↓
Accept Order
      ↓
Enter OTP
      ↓
Complete Delivery
```

---

## ✨ Features

### 👤 Customer Management
- Create a customer profile
- Store customer name, phone number and address
- Maintain wallet balance
- Add money to the customer wallet

### 🍽️ Restaurant & Menu
- Restaurant information
- Multiple menu items
- Veg / Non-Veg classification
- Display item prices
- Interactive menu selection

### 🛒 Order Management
- Select multiple food items
- Place an order
- Automatically generate an Order ID
- Calculate:
  - Subtotal
  - GST
  - Packaging fee
  - Total bill
- Display estimated delivery time
- Track order status

### 🛵 Delivery Partner
- Create a delivery partner
- Store phone number and vehicle details
- Track availability
- Accept customer orders

### 🔐 OTP Verification
- Generate an order OTP
- Verify OTP before delivery
- Prevent delivery with an incorrect OTP

### 📦 Delivery Tracking
Order status progresses through the delivery workflow:

```text
Placed → Accepted → Delivered
```

### 🌐 Streamlit Interface
- Clean and simple web interface
- Interactive forms and buttons
- Session state for maintaining application data
- Real-time order and delivery status

---

## 🧠 OOP Concepts Demonstrated

The project is designed to demonstrate important Object-Oriented Programming concepts.

| OOP Concept | Implementation |
|---|---|
| **Class & Object** | `Customer`, `Restaurant`, `Order`, `MenuItem`, `DeliveryPartner` |
| **Inheritance** | `Customer` and `DeliveryPartner` inherit from `User` |
| **Abstraction** | `User` uses abstract methods |
| **Encapsulation** | Internal attributes such as wallet balance and order status |
| **Polymorphism** | `notify()` and `display_profile()` are implemented by different subclasses |
| **Methods** | Order placement, wallet management, OTP verification and delivery |

---

## 🏗️ Project Structure

```text
Food-Delivery/
│
├── app.py
├── food_delivery.py
├── streamlit_app.py
├── Food_Delivery_System_Not


