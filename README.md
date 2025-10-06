
# Shopease – Modern Full-Stack E-Commerce Platform

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)  
[![Java](https://img.shields.io/badge/Java-JDK%208%2B-orange.svg)](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html)  
[![MySQL](https://img.shields.io/badge/MySQL-8.0-blue.svg)](https://www.mysql.com/)  
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-purple.svg)](https://getbootstrap.com/)

Shopease is a **full-stack E-Commerce platform** built with **Java, JSP, Servlets, JDBC, MySQL, and Bootstrap 5**, designed to provide a seamless shopping experience for users and efficient product management for admins. Users can browse, search, filter, and purchase electronic products online, while admins manage inventory and orders effectively.

---

## **Features**

### **User Features**
- Secure **registration and login**.
- Browse, **search**, and **filter products** by category.
- Add multiple products to **shopping cart**, adjust quantities, and proceed to checkout.
- Simulate **credit card payments** for demo orders.
- Track orders and view **shipment status**.
- Receive **automated email notifications** for registration, orders, stock updates, and shipment alerts.

### **Admin Features**
- Add, update, or remove products from the store.
- Manage **inventory** with real-time updates.
- Track all orders and **mark them as shipped or delivered**.
- Optional: **Sales analytics** dashboard for admin insights.

---

## **Technologies Used**
- **Front-End:** HTML, CSS, JavaScript, Bootstrap 5  
- **Back-End:** Java (Servlets, JSP), JDBC  
- **Database:** MySQL  
- **Build & Deployment:** Maven, Tomcat 8+  
- **Email Notifications:** Gmail API  

---

## **Setup Instructions**

### **1. Clone the Repository**
```bash
git clone https://github.com/<your-username>/shopease.git
````

### **2. Configure Database**

1. Open MySQL Workbench or Command Prompt.
2. Login:

```sql
mysql -u <username> -p
```

3. Run the database script: `databases/mysql_query.sql`
4. Update `application.properties` with your MySQL credentials:

```properties
db.username=<your_mysql_user>
db.password=<your_mysql_password>
```

### **3. Configure Email (Gmail)**

1. Enable **2-step verification** on your Gmail account.
2. Generate **App Password**: [Gmail App Passwords](https://myaccount.google.com/apppasswords)
3. Update `application.properties`:

```properties
mailer.email=<your_email>
mailer.password=<app_password>
```

### **4. Import and Build Project**

1. Open **Eclipse EE** → File → Import → Git → Projects from Git → Clone URI → Paste repository URL.
2. Right-click project → **Run as → Maven build** → Goals: `clean install`
3. Resolve any missing libraries or dependencies.

### **5. Configure Tomcat Server**

1. Right-click project → **Run As → Run on Server** → Select Tomcat 8+ → Add project → Finish
2. Open browser: `http://localhost:8080/shopease/`

### **6. Default Credentials**

* **Admin:** `admin@gmail.com` / `admin`
* **User:** `guest@gmail.com` / `guest`

---

## **Project Highlights**

* Full **user and admin management**.
* **Automated email notifications** for key events.
* **Responsive modern UI** with Bootstrap 5.
* Demo **credit card payment flow** for checkout simulation.
* **MVC architecture** with clean and maintainable Java code.

---

## **Future Enhancements**

* Integrate **real payment gateway** (Stripe/PayPal).
* Add **product reviews and ratings**.
* Implement **AJAX-based cart and live search**.
* Add **analytics dashboard** for admins with charts using Chart.js.

---

## **License**

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details. 

