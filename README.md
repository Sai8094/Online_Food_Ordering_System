# 🍴 Online Food Ordering System (Java)

A reference implementation of an **Online Food Ordering System** in Java, designed using **SOLID principles** and classical design patterns:  
- **Singleton** for database connection management  
- **Factory** for creating food items (`Pizza`, `Burger`, `Drinks`)  
- **Abstract Factory** for cuisine-specific items (`ItalianFactory`, `IndianFactory`)  
- **Builder** for constructing complex orders with multiple customizations  
- **Observer** for notifying customers about order status updates  
- **Strategy** for applying different payment methods (`CreditCard`, `UPI`, `PayPal`)  

## ✨ Features

- Centralized **DatabaseConnection** (singleton) for consistent DB access  
- Food item creation with **Factory Pattern**  
- Region/cuisine-specific menus via **Abstract Factory**  
- Flexible order building with add-ons, sides, and drinks (**Builder**)  
- Real-time **Order Status Notifications** (Observer)  
- Multiple **Payment Strategies** (plug-and-play for different gateways)  

## 🧠 SOLID Principles Mapping

- **S**ingle Responsibility → Each class has a single responsibility (e.g., `CustomerObserver` only manages notifications).  
- **O**pen/Closed → Extend system (add new cuisines, food items, payment types) without modifying existing code.  
- **L**iskov Substitution → All subclasses (`Pizza`, `Burger`, `Drink`) behave as `FoodItem`.  
- **I**nterface Segregation → Small interfaces (`OrderObserver`, `PaymentStrategy`) instead of large ones.  
- **D**ependency Inversion → High-level modules depend on abstractions (`PaymentStrategy`, `CuisineFactory`) not implementations.  
