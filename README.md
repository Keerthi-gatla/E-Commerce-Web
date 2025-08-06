# 🛒 E-Commerce Web Application

This is a full-stack **E-Commerce Web Application** built with modern technologies including **React**, **Spring Boot**, **MySQL**, and **Amazon AWS S3** for image storage. The platform enables users to browse products, manage their cart, and simulate an order checkout flow — all connected through a robust RESTful API backend.

---

## 🧰 Tech Stack

- **Frontend:**
  - React.js
  - HTML5, CSS3

- **Backend:**
  - Java
  - Spring Boot
  - RESTful APIs

- **Database:**
  - MySQL (via SQL Workbench)

- **Cloud:**
  - Amazon AWS S3 (for product image storage)

---

## 📦 Features

- 🔍 Product listing with image preview
- 🛒 Add to Cart & View Cart
- ✅ Checkout simulation
- 🧾 Order Summary
- 🔐 Secure API interaction
- ☁️ Image storage via AWS S3
- 🧠 Clean and scalable architecture (frontend ↔ backend ↔ database)

---

## 📂 Project Structure

```

/ecommerce-project
│
├── /frontend     → React app
└── /backend      → Spring Boot API + DB layer

````

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/keerthi-gatla/ecommerce-project.git
cd ecommerce-project
````

---

### 2. Backend Setup (`/backend` - Spring Boot)

> Prerequisites: Java 17+, Maven, MySQL installed

* Import the `/backend` folder into IntelliJ, Eclipse, or Spring Tool Suite
* Update your `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
spring.datasource.username=your_username
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update

aws.access-key=YOUR_AWS_ACCESS_KEY
aws.secret-key=YOUR_AWS_SECRET_KEY
aws.s3.bucket-name=your-s3-bucket-name
```

* Run the backend:

```bash
mvn spring-boot:run
```

---

### 3. Frontend Setup (`/frontend` - React)

> Prerequisites: Node.js + npm or yarn

```bash
cd frontend
npm install
npm start
```

Frontend runs by default on: [http://localhost:3000](http://localhost:3000)

---

### 4. Database Setup

* Create a database using **MySQL Workbench**:

```sql
CREATE DATABASE ecommerce_db;
```

* Spring Boot will auto-generate tables on first run (thanks to `hibernate.ddl-auto=update`)
* Optional: Use a `.sql` dump if provided for sample data

---

## 🖼️ Image Handling via AWS

* Product images are stored on **Amazon S3 buckets**
* The backend includes functionality to upload and fetch image URLs from AWS
* Make sure to configure correct **IAM permissions** for the S3 bucket

---

## 🤝 Contact & Contributions

* 📧 Email: [keerthi.ece.software@gmail.com](mailto:keerthi.ece.software@gmail.com)
* 🧑‍💻 GitHub: [keerthi-gatla](https://github.com/keerthi-gatla)

Feel free to fork, clone, or contribute!
For collaboration or queries, contact via email above.

---

## 📄 License

This project is open-source and available under the **MIT License**.

---

## 🙌 Acknowledgements

* ReactJS Docs
* Spring Boot Guides
* MySQL Community
* AWS S3 Documentation

