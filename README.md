<!-- Banner -->
<p align="center">
  <img src="[https://images.unsplash.com/photo-1526378722484-cc5c510f9f3d?auto=format&fit=crop&w=1400&q=80](https://images.wallpaperscraft.com/image/single/gradient_color_shades_140497_3840x2160.jpg)" 
       alt="Backend Project Banner" width="100%">
</p>

<h1 align="center">🛒 Product Management Backend</h1>
<p align="center">
  A <b>Spring Boot REST API</b> for managing products with CRUD operations, image handling, and database integration.  
</p>

---

## 🚀 Features
- 📦 **Product Management** – Create, update, delete, and fetch products.  
- 🖼️ **Image Upload & Retrieval** – Store and serve images directly via REST endpoints.  
- 🗄️ **Database Integration** – JPA Repository support for persistence.  
- ⚡ **Lightweight & Scalable** – Built on Spring Boot with RESTful principles.  

---

## 🛠️ Tech Stack
- **Java 17+**  
- **Spring Boot** (Web, JPA)  
- **MySQL / PostgreSQL** (configurable)  
- **Maven** for dependency management  

---

## 📂 Project Structure
```bash
├── controller
│   └── ProductController.java
├── service
│   └── ProductService.java
├── repository
│   └── ProductRepo.java
└── model
    └── Product.java
```

---

## 🔑 API Endpoints

| Method | Endpoint                   | Description                  |
|--------|-----------------------------|------------------------------|
| POST   | `/product`                  | Create new product with image |
| GET    | `/product/{id}`             | Get product details by ID     |
| GET    | `/product/{id}/image`       | Fetch product image           |
| PUT    | `/product/{id}`             | Update product details        |
| DELETE | `/product/{id}`             | Delete product                |

---

## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/shanmugapandiyan/E-Commerce-Application.git
   cd product-backend
   ```

2. **Configure Database**  
   Update `application.properties` with your DB credentials:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/productdb
   spring.datasource.username=root
   spring.datasource.password=yourpassword
   ```

3. **Build & Run**
   ```bash
   mvn spring-boot:run
   ```

---

## 🎯 Usage Example (Image Upload with cURL)

```bash
curl -X POST http://localhost:8080/product  -F "p={\"name\":\"Laptop\",\"price\":75000}"  -F "image=@/path/to/laptop.png"
```

---

## 📸 Screenshots



---

## 🌟 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

---

## 📜 License
This project is licensed under the MIT License – feel free to use and modify.

---

<p align="center">💻 Built with ❤️ using Spring Boot</p>
