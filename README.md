#  Update and Search Products/Buyers – Java Swing Application

This project implements **Update and Search functionalities** for managing **Products and Buyers** using a **Java Swing GUI** and **MySQL database**. It is part of a larger inventory/customer management system and fulfills all the requirements outlined in **Task 6 of the project documentation**.

---

*COMPANY*: Main Flow Services and Technologies Pvt. Ltd. 

*NAME* : shiva kasula

*INTERN ID* : 17203

*DOMAIN* : Full Stack Web Development

*DURATION* : 8WEEKS

## 📌 Features Implemented

### ✅ Product Update Functionality
- Search product by ID
- Prefilled update form with existing product details
- Fields: Name, Category, Price, Quantity, Description
- Update button commits changes to the database
- Input validation and error handling included
- Admin-only access to update forms

### ✅ Buyer (Customer) Update Functionality
- Update customer details via a form (Admin access only)
- Editable fields: Name, Gender, Email, Phone, Address
- Pre-fill on search by Customer ID
- Update logic includes validation and database update query

### ✅ Product Search Interface (Customer Side)
- Dynamic search by **Product Name** or **Category**
- Case-insensitive and partial match supported
- Table highlights matched terms
- Results shown in a JTable with:
  - `ID`, `Name`, `Category`, `Price`, `Quantity`, `Description`
- Product details shown in a separate text area on row click

### ✅ Reset Functionality
- Clears search field and table filters
- Clears product detail view
- Reloads full product list

### ✅ Logout Function
- Returns user to the login screen
- Confirmation popup for exit

---

## 📁 Project Structure

<pre>
ProductCustomer/
├── src/
│   └── main/
│       └── java/
│           └── com/mycompany/productcustomer/
│               ├── AdminHome.java
│               ├── UpdateProduct.java
│               ├── UpdateCustomer.java
│               ├── CustomerHome.java
│               ├── DeleteCustomer.java
│               ├── LoginForm.java
│               ├── DatabaseConnection.java
│               └── ... (other modules)
├── pom.xml              # Maven configuration file
├── README.md            # Project documentation
└── testdb.sql           # MySQL database dump file
</pre>




---

## 🧰 Technologies Used

| Component       | Description                      |
|----------------|----------------------------------|
| Java            | Core language (Java 17+/JDK 24) |
| Swing GUI       | Desktop interface framework     |
| MySQL           | Backend RDBMS                   |
| JDBC            | Java Database Connectivity      |
| NetBeans IDE    | Development environment         |
| Maven           | Dependency & project management |

---

## 🚀 How to Run

1. **Clone the Repository**
```bash
git clone https://github.com/your-username/ProductCustomer.git
cd ProductCustomer
```
## 🚀 Project Setup Instructions

### 🧩 Import into NetBeans

1. Open **NetBeans**.
2. Click on **File → Open Project**.
3. Navigate to the project folder and select it (e.g., `ProductCustomer`).
4. Wait for dependencies to load.

---

### 🗄️ Configure the Database

1. Open **phpMyAdmin** or any MySQL client.
2. Create a new database named:**testdb**
3. 
3. Import `testdb.sql` if it exists in your project directory.

---

### 🔑 Update Database Credentials

Open the file:

```bash
src/main/java/com/mycompany/productcustomer/DatabaseConnection.java
```


Update the credentials if necessary:

```java
String url = "jdbc:mysql://localhost:3306/testdb";
String username = "root";
String password = ""; // Use your MySQL password if any
```

### ▶️ Run the Application

1. Open the project in **NetBeans**.
2. Make sure the database `testdb` is running in MySQL.
3. Ensure you’ve imported `testdb.sql` if provided.
4. If required, update the DB credentials in: `src/main/java/com/mycompany/productcustomer/DatabaseConnection.java

5. In the **Projects** pane:
- Navigate to:  
  `src → main → java → com.mycompany.productcustomer → LoginForm.java`
- **Right-click** on `LoginForm.java` and select:
  ```
  Run File
  ```

6. The application GUI will launch.

---

### 👤 Login Details

- **Admin Login:**  
➤ Full access to **Add, Update, Delete** products or customers

- **Customer Login:**  
➤ Can **Search and View** products only

## 🖼️ Screenshots

### 🔐 Login Page
![Login Page]<img width="598" height="519" alt="Image" src="https://github.com/user-attachments/assets/80bee57b-fdcc-4b50-a6c4-68b8448b1a15" />

---

### 🧑 Admin - Update Product
![Admin - Update Product](screenshots/admin-update-product.png)

---

### 🔍 Customer - Product Search
![Customer - Product Search](screenshots/customer-product-search.png)





