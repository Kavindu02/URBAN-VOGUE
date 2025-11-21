# 👗 URBAN VOGUE

> A modern, full-featured clothing e-commerce website - My first web development project!

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=flat&logo=css3&logoColor=white)
![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=flat&logo=php&logoColor=white)
![Status](https://img.shields.io/badge/status-active-success.svg)

## 📋 Overview

Urban Vogue is a comprehensive clothing e-commerce platform that provides a seamless shopping experience for fashion enthusiasts. This project marks the beginning of my web development journey, featuring a complete online store with user authentication, product management, shopping cart, and order tracking.

## ✨ Features

### 🛍️ Customer Features
- **Browse Products**: Explore a wide range of clothing items with detailed descriptions
- **Product Details**: View comprehensive product information, images, and pricing
- **Shopping Cart**: Add items to cart and manage quantities
- **User Authentication**: Secure sign-up and login system
- **Order Tracking**: Track your orders from purchase to delivery
- **Purchase History**: View all previous purchases and transactions
- **User Profile**: Manage personal information and preferences
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices

### 👨‍💼 Admin Features
- **Admin Dashboard**: Comprehensive control panel for store management
- **Product Management**: Add, edit, and delete products
- **Order Management**: View and process customer orders
- **User Management**: Monitor and manage user accounts
- **Inventory Control**: Track stock levels and product availability

### 📄 Additional Pages
- **About Us**: Learn about Urban Vogue's story and mission
- **Privacy Policy**: Detailed privacy and data protection information
- **Terms & Conditions**: Clear terms of service and usage policies

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3
- **Backend**: PHP
- **Database**: MySQL (assumed from PHP usage)
- **Architecture**: Multi-page application with separate user and admin interfaces

## 📁 Project Structure

```
URBAN-VOGUE/
├── Product Details/
│   └── (Product detail pages and assets)
│
├── Pages/
│   ├── Customer Pages
│   ├── About.html
│   ├── About css.css
│   ├── Home Page.html
│   ├── Home Page css.css
│   ├── product page.html
│   ├── product page css.css
│   ├── profile.html
│   ├── profile css.css
│   ├── Purchase History.html
│   ├── Purchase History css.css
│   ├── Order tracking.html
│   ├── order tracking css.css
│   ├── Privacy Policy.html
│   ├── Privacy Policy css.css
│   ├── Terms and Condition.html
│   ├── Term and Condition css.css
│   │
│   ├── Shopping Cart
│   ├── Add to cart.html
│   ├── Add to cart css.css
│   │
│   ├── Authentication
│   ├── loginPage.php.php
│   ├── Sign up Page.php.php
│   ├── User Login Page.html
│   ├── User Login Page css.css
│   ├── User Sign up page.html
│   └── User Sign up Page css.css
│
├── Admin Panel
│   ├── Admin page.html
│   ├── Admin page.php.php
│   └── Admin page css.css
│
└── desktop.ini
```

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:
- **Web Server**: Apache, Nginx, or any PHP-compatible server
- **PHP**: Version 7.4 or higher
- **MySQL**: Version 5.7 or higher
- **Web Browser**: Chrome, Firefox, Safari, or Edge

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/urban-vogue.git
   cd urban-vogue
   ```

2. **Set up your web server**
   
   For **XAMPP** (Recommended for beginners):
   - Download and install [XAMPP](https://www.apachefriends.org/)
   - Copy the project folder to `htdocs` directory
   - Start Apache and MySQL from XAMPP Control Panel

   For **WAMP**:
   - Download and install [WAMP](https://www.wampserver.com/)
   - Copy the project folder to `www` directory
   - Start WAMP server

3. **Set up the database**
   
   Create a new MySQL database:
   ```sql
   CREATE DATABASE urban_vogue;
   USE urban_vogue;
   
   -- Import your SQL file if you have one
   -- Or create tables as needed
   ```

4. **Configure database connection**
   
   Update your PHP configuration files with database credentials:
   ```php
   <?php
   $servername = "localhost";
   $username = "root";
   $password = "";
   $dbname = "urban_vogue";
   
   $conn = new mysqli($servername, $username, $password, $dbname);
   ?>
   ```

5. **Access the application**
   
   Open your web browser and navigate to:
   ```
   http://localhost/urban-vogue/Home Page.html
   ```
   
   For admin panel:
   ```
   http://localhost/urban-vogue/Admin page.html
   ```

## 🎨 Pages Overview

### Customer Interface
- **Home Page**: Landing page with featured products and categories
- **Product Page**: Browse all available clothing items
- **Product Details**: Detailed view of individual products
- **Shopping Cart**: Review and manage cart items
- **User Profile**: Personal account management
- **Order Tracking**: Real-time order status updates
- **Purchase History**: Complete order history
- **About Us**: Company information and story
- **Privacy Policy**: Data protection and privacy information
- **Terms & Conditions**: Legal terms and conditions

### Authentication
- **Login Page**: Secure user authentication
- **Sign Up Page**: New user registration with validation

### Admin Interface
- **Admin Dashboard**: Centralized management panel
- **Product Management**: CRUD operations for products
- **Order Management**: Process and track orders
- **User Management**: Monitor user accounts

## 🔐 Security Features

- Password encryption for user accounts
- SQL injection prevention
- XSS (Cross-Site Scripting) protection
- Session management for secure authentication
- Admin access control

## 📱 Responsive Design

Urban Vogue is fully responsive and works seamlessly on:
- 🖥️ Desktop (1920px and above)
- 💻 Laptop (1024px - 1919px)
- 📱 Tablet (768px - 1023px)
- 📱 Mobile (320px - 767px)

## 🌐 Browser Compatibility

- ✅ Google Chrome (latest)
- ✅ Mozilla Firefox (latest)
- ✅ Microsoft Edge (latest)
- ✅ Safari (latest)
- ✅ Opera (latest)

## 🚀 Deployment

### Deploy to Shared Hosting

1. Export your database from phpMyAdmin
2. Upload files via FTP to your hosting provider
3. Import database to hosting server
4. Update database connection settings
5. Test all functionality

### Deploy to Cloud Platforms

#### Heroku
1. Install Heroku CLI
2. Create a new Heroku app
3. Add MySQL addon (JawsDB or ClearDB)
4. Push your code to Heroku

#### AWS
1. Set up EC2 instance
2. Install LAMP stack
3. Configure security groups
4. Deploy your application

## 📊 Database Schema (Example)

```sql
-- Users Table
CREATE TABLE users (
    user_id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(50) UNIQUE NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    password VARCHAR(255) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Products Table
CREATE TABLE products (
    product_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    description TEXT,
    price DECIMAL(10, 2) NOT NULL,
    stock INT DEFAULT 0,
    category VARCHAR(50),
    image_url VARCHAR(255)
);

-- Orders Table
CREATE TABLE orders (
    order_id INT PRIMARY KEY AUTO_INCREMENT,
    user_id INT,
    order_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    total_amount DECIMAL(10, 2),
    status VARCHAR(20),
    FOREIGN KEY (user_id) REFERENCES users(user_id)
);

-- Cart Table
CREATE TABLE cart (
    cart_id INT PRIMARY KEY AUTO_INCREMENT,
    user_id INT,
    product_id INT,
    quantity INT DEFAULT 1,
    FOREIGN KEY (user_id) REFERENCES users(user_id),
    FOREIGN KEY (product_id) REFERENCES products(product_id)
);
```

## 🎯 Future Enhancements

- [ ] Payment gateway integration (PayPal, Stripe)
- [ ] Email notifications for orders
- [ ] Product reviews and ratings
- [ ] Wishlist functionality
- [ ] Advanced search and filters
- [ ] Size and color variants
- [ ] Discount coupons system
- [ ] Social media integration
- [ ] Live chat support
- [ ] Multiple language support
- [ ] Product recommendations
- [ ] Inventory alerts for admins

## 🤝 Contributing

This is my first project, and I'm open to suggestions and improvements!

If you'd like to contribute:
1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Learning Journey

### What I Learned Building This Project:

- ✅ HTML5 semantic markup and structure
- ✅ CSS3 styling, layouts, and responsive design
- ✅ PHP server-side programming
- ✅ MySQL database design and queries
- ✅ User authentication and session management
- ✅ CRUD operations (Create, Read, Update, Delete)
- ✅ Form validation and data sanitization
- ✅ E-commerce workflow and logic
- ✅ Admin panel development
- ✅ Project structure and organization

### Challenges Faced:

- Understanding PHP-MySQL integration
- Implementing secure authentication
- Creating responsive layouts
- Managing shopping cart logic
- Handling file uploads for product images

## 👨‍💻 Author

Kavindu Rathnayaka
