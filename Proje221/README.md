# 🎟️ Event Management System (Java)

A **Java-based Event Management System** built using **Object-Oriented Programming (OOP)** principles. The system allows administrators to manage events and users to browse events and purchase tickets. This project is designed for **learning, academic purposes, and technical interviews**.

---

## 📌 Project Overview

This project simulates a real-world **event & ticket management platform**. Different event types such as **Concerts**, **Conferences**, and **Sports Events** are modeled using inheritance, while users can purchase **VIP or standard tickets** with seat validation and discounts.

The focus of this project is on:
- Clean OOP design
- Proper use of inheritance and abstraction
- Realistic business logic (VIP pricing, seat limits, discounts)

---

## 🛠️ Technologies Used

- **Java**
- **Java Swing** (GUI for menus & interactions)
- **Collections Framework** (ArrayList, HashMap, HashSet)

---

## 🧱 Project Structure

```
src/
├── Event/
│   └── Event.java               # Abstract base class for all events
│
├── Event_is_a/
│   ├── Concert.java             # Concert event type
│   ├── Conference.java          # Conference event type
│   └── SportsEvent.java         # Sports event type
│
├── Ticket/
│   └── Ticket.java              # Ticket model (VIP / standard)
│
├── User/
│   └── User.java                # User model (admin, student, normal)
│
├── has_a/
│   └── Identifiable.java        # Interface for unique IDs
│
├── sys/
│   └── EventManagementSystem.java  # Core system logic
│
├── main/
│   └── EventManagementMain.java # Application entry point
│
└── GUI/
    └── MainMenuFrame.java       # Swing-based GUI (not shown here)
```

---

## 🧩 Core Design & OOP Concepts

### 🔹 Abstraction
- `Event` is an **abstract class** defining common event properties.
- Each event type implements its own `displayEventDetails()` method.

### 🔹 Inheritance (IS-A relationship)
- `Concert`, `Conference`, and `SportsEvent` **extend** the `Event` class.

### 🔹 Interface (HAS-A / Contract)
- `Identifiable` interface ensures every entity has a unique ID.
- Implemented by `Event`, `Ticket`, and `User`.

### 🔹 Polymorphism
- Events are stored as `ArrayList<Event>` and handled dynamically.

---

## ✨ Features

### 🎫 Event Management
- Add and delete events
- Auto-generated unique event IDs
- Support for multiple event types

### 🪑 Ticket System
- VIP and Standard tickets
- Seat number validation
- Prevents double booking of seats
- VIP tickets cost **2× price**

### 🎓 Discounts
- **Student users** receive a discount on VIP tickets

### 👤 User Roles
- **Admin** – manages events
- **Student** – receives discounts
- **Normal User** – standard access

### 📊 Revenue Tracking
- Calculates total revenue from sold tickets

---

## ▶️ How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/event-management-system.git
   ```

2. Open the project in an IDE (IntelliJ IDEA / Eclipse)

3. Run:
   ```
   EventManagementMain.java
   ```

4. The GUI menu will appear

---

## 🧪 Sample Data

The system automatically creates:
- Test users (admin, student, normal)
- Sample events (concerts, conferences, sports events)

This allows quick testing without manual setup.

---

## 📸 Screenshots (Optional)

_Add screenshots of the GUI here if available._

---

## 🚀 Future Improvements

- Persistent storage (database or file system)
- Authentication & login screen
- Ticket cancellation
- Improved GUI design
- REST API version

---

## 👨‍💻 What This Project Demonstrates

- Strong understanding of **OOP concepts**
- Clean separation of responsibilities
- Real-world problem modeling
- Java collections & data structures

This project is ideal for **junior Java developer interviews** and academic submissions.

---

## 📄 License

This project is for educational purposes.

