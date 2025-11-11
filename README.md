# Smart-Inventory-MS
Smart Inventory Management System

A Java + Hibernate-based desktop application designed to simplify and automate the process of inventory tracking, stock management, and supplier control.
This system helps businesses efficiently manage product details, purchases, and sales while maintaining real-time stock levels and generating insightful reports.

🚀 Features

✅ User-Friendly Interface – Simple and intuitive GUI built using Java Swing/JavaFX.
✅ Product Management – Add, update, delete, and view product details with quantity, price, and category.
✅ Supplier Management – Maintain supplier records for tracking purchase sources.
✅ Stock Monitoring – Automatic stock updates after sales and purchases.
✅ Sales & Purchase Records – Manage all transactions with timestamps and bill references.
✅ Low Stock Alerts – Get alerts when stock falls below threshold.
✅ Search & Filter – Quickly find products, suppliers, or transactions.
✅ Reports & Analytics – Generate summaries of sales, purchases, and stock.
✅ Database Integration (Hibernate) – Uses Hibernate ORM for smooth data handling and database operations.

🏗️ Tech Stack
Layer	Technology Used
Language	Java (JDK 8 or above)
ORM Framework	Hibernate
Database	MySQL (or H2 for testing)
UI Framework	Java Swing / JavaFX
Build Tool	Maven / Gradle
Logging	Log4j (optional)
🧩 Project Structure
SmartInventory/
│
├── src/main/java/com/inventory/
│   ├── dao/                # Data Access Objects (Hibernate operations)
│   ├── model/              # Entity classes (Product, Supplier, Sales, etc.)
│   ├── service/            # Business logic
│   ├── util/               # Hibernate utility & config
│   ├── ui/                 # Swing/JavaFX forms
│   └── Main.java           # Application entry point
│
├── src/main/resources/
│   ├── hibernate.cfg.xml   # Hibernate configuration file
│   └── log4j.properties    # (Optional) logging configuration
│
├── pom.xml                 # Maven dependencies
├── README.md               # Project documentation
└── database.sql            # Sample database schema

⚙️ Installation & Setup
🔧 Prerequisites

Java JDK 8 or above

MySQL Server (or H2 database for testing)

Maven or Gradle

IDE (IntelliJ IDEA, Eclipse, or NetBeans)

🧭 Steps to Run

Clone the Repository:

git clone https://github.com/your-username/SmartInventory.git
cd SmartInventory


Configure Database:

Create a database named inventory_db in MySQL.

Import the database.sql file provided.

Update hibernate.cfg.xml with your DB credentials:

<property name="hibernate.connection.url">jdbc:mysql://localhost:3306/inventory_db</property>
<property name="hibernate.connection.username">root</property>
<property name="hibernate.connection.password">yourpassword</property>


Build the Project:

mvn clean install


Run the Application:

java -jar target/SmartInventory.jar


or run Main.java directly from your IDE.

📊 Database Design

Main Tables:

product – Stores product details (id, name, category, quantity, price).

supplier – Supplier info (id, name, contact).

purchase – Tracks all purchases and updates stock.

sales – Logs all sales transactions.

user – (Optional) For login/authentication.

🧠 Future Enhancements

Add user authentication (admin, staff roles)

Integrate barcode scanning

Enable REST API backend for web or mobile apps

Add Excel/PDF export of reports

Implement email/SMS alerts for low stock
