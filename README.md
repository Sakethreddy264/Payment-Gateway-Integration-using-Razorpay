💳 Razorpay Payment Gateway Integration with Spring Boot
This is a full-stack project that demonstrates how to integrate Razorpay Payment Gateway with a Java Spring Boot backend. It includes secure order creation, Razorpay Checkout integration, and a modern user-friendly frontend.

🚀 Features
📦 Create Razorpay orders from the backend

💰 Accept secure payments using Razorpay Checkout

🛠 Save and update order/payment data using JPA & MySQL

✅ Callback handling to mark orders as "PAID"

🌐 Clean, responsive UI using HTML + Bootstrap 5

🛠 Tech Stack
Backend: Java 21, Spring Boot 3, Spring Web, JPA, HikariCP

Frontend: HTML5, Bootstrap 5, Razorpay Checkout.js

Database: MySQL

Payment API: Razorpay Java SDK

⚙️ Setup Instructions
1. Clone the Repository
bash
git clone https://github.com/yourusername/razorpay-springboot-integration.git
cd razorpay-springboot-integration
2. Create MySQL Database
sql
CREATE DATABASE razorpay_db;
3. Configure Application Properties
Update src/main/resources/application.properties:

properties
spring.datasource.url=jdbc:mysql://localhost:3306/razorpay_db
spring.datasource.username=your_db_username
spring.datasource.password=your_db_password

razorpay.key_id=YOUR_KEY_ID
razorpay.key_secret=YOUR_KEY_SECRET
4. Run the Application
bash
./mvnw spring-boot:run
🌐 Access the App
Frontend Page: http://localhost:8080/orders.html

Success Page: Automatically redirects after payment

📂 Project Structure
src/
├── main/
│   ├── java/com/spring/implementation/
│   │   ├── controller/
│   │   ├── model/
│   │   ├── repository/
│   │   └── service/
│   └── resources/
│       ├── static/
│       │   ├── orders.html
│       │   └── success.html
│       └── application.properties
