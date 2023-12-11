# Design Document for Crimson Mart Web Application

The Crimson Mart web application, developed using HTML, CSS, JavaScript, Bootstrap for the front end, Python with Flask for the back end, and SQL for database queries, aims to provide a user-friendly marketplace for buying and selling products. Users can seamlessly navigate through product listings, manage their carts, execute purchases, and also list their products for sale. This comprehensive platform caters to both buyers and sellers, facilitating transactions and interactions between them. Below is a comprehensive overview of its architecture, technologies used,and implementation decisions.

## Architecture and Technologies

### Flask Framework

- **Routing and Views:** The application utilizes Flask's robust routing system to handle HTTP requests and render dynamic pages using Jinja2 templating.
- **Session Management:** Flask-Session enables efficient session handling, maintaining user-specific data across requests for enhanced usability.

### Database - SQLite

- **CS50 Library:** Database operations are managed using the cs50 library, utilizing SQL queries to handle user data, product listings, and cart items.
- **Database Schema:** The SQLite database includes tables for users, products, and cart items, storing essential details like user information, product descriptions, and pricing.

### Frontend - HTML, CSS, JavaScript, Bootstrap

- **Templates and Styling:** HTML templates populated dynamically with backend data alongside CSS and Bootstrap ensure a responsive and visually appealing user interface.
- **Interactive Elements:** JavaScript enhances user interactions, facilitating actions like adding items to the cart without page reloads.

### File Uploads

- **Upload Handling:** Secure file uploads for product images are managed using werkzeug.utils, storing them in the static/img/product_img folder.

## Implementation Decisions

### Security Measures

- **Password Hashing:** User passwords are securely hashed using werkzeug.security before storage, ensuring sensitive data remains protected.
- **Session Security:** Flask sessions are employed for user authentication, mitigating unauthorized access risks.

### Error Handling

- **Flash Messages:** Flash messages notify users of successful actions or errors, enhancing the overall user experience.

### Code Structure

- **Modularization:** Codebase is logically structured into routes for different functionalities (e.g., login, registration, product listings), promoting readability and maintainability.

## Additional Information

In the Crimson Mart project, Flask routing was implemented, utilizing the static folder to store CSS, fonts, images, and JavaScript files. HTML files were stored in the template folder, and the backend was handled via app.py. The database, named crimsonmart.db, includes tables for users, cart, and products.



## Conclusion

Crimson Mart successfully implements a robust marketplace using Flask and a blend of technologies, prioritizing security, usability, and maintainability.