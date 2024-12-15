[TOC]

## Common Functional Requirements for the E-shop System:

1. **Product Catalog Management**:
   - The system must allow the addition, deletion, and modification of products in the catalog (e.g., electronics, wearables, phones, etc.).
   - Products must be categorized, and each category must have attributes (e.g., brand, model, price, features).
2. **Inventory Management**:
   - The system must track the quantity of each product available in stock.
   - The system must generate alerts when stock is low for specific products.
3. **Customer Management**:
   - The system must manage customer profiles, including their order history, preferences, and addresses.
   - There should be user registration and login functionality.
4. **Order Processing**:
   - Customers must be able to place orders for products.
   - The system must process and confirm orders, including real-time payment processing and shipping arrangements.
5. **Payment Gateway Integration**:
   - The system must be integrated with payment gateways (e.g., PayPal, credit cards) to handle secure transactions.
6. **Search and Filter Functionality**:
   - Customers must be able to search for products based on keywords and filter products by criteria such as price, brand, and ratings.
7. **Recommendation System**:
   - The system should offer personalized product recommendations based on user browsing behavior or past purchases.
8. **Analytics and Reporting**:
   - The system should provide insights into sales performance, customer behavior, and popular products.
   - Admins should be able to generate reports on inventory, orders, and customer activity.
9. **Security and User Authentication**:
   - Secure login and password protection for customers and administrators.
   - Protection against common cyber threats (e.g., SQL injection, phishing).
10. **Responsive Design**:
    - The system must be accessible on various devices, including desktops, smartphones, and tablets.

### **Non-functional Requirements**:

1. **Scalability**:
   - The system must handle growing user traffic, especially during sales seasons.
2. **Performance**:
   - Page loading times must be minimal, with a goal of loading within 3 seconds even under peak traffic.
3. **Reliability**:
   - The system should have an uptime of at least 99.9%.
4. **Security**:
   - All sensitive data (such as payment and personal information) must be encrypted.
   - The system must comply with relevant data protection regulations (e.g., GDPR).
5. **Usability**:
   - The interface should be intuitive for both tech-savvy and non-tech-savvy users.

### Topics

1. **Information Systems**:
   - **Typical situations**: For example, determining which products need to be restocked (inventory management), or analyzing customer behavior for marketing (analytics and reporting).
   - **Relevant information**: Product inventory levels, customer purchase history, and financial reports.
   - **Information system components**: The backend (databases), the frontend (user interface), and middleware (business logic for managing orders, payments, etc.).
2. **Database Systems**:
   - **What to store**: Product data (e.g., name, description, stock levels), customer profiles, and order details.
   - **Benefits of using a database**: Data consistency, easier querying, and enhanced security (vs. file-based storage).
   - **Database structure**: Entities like "Product," "Customer," and "Order" with attributes such as product name, customer email, etc.
   - **Typical database operations**: Checking stock levels, retrieving customer orders, and generating reports.
3. **Algorithms and Programming**:
   - **Problem-solving example**: How to design an efficient search and filter algorithm for products.
   - **Algorithm design**: Sorting algorithms for showing products by price or popularity.
   - **Implementation example**: Writing a sorting or recommendation algorithm in Python/Java/C# that takes user preferences and displays relevant products.
4. **Artificial Intelligence**:
   - **Applications of AI**: Personalized product recommendations, automated customer service via chatbots, and fraud detection in payments.
   - **Intelligent behavior**: Product recommendations based on browsing patterns can be considered intelligent because they adjust based on user behavior (learning through data).
   - **Learning application**: Machine learning models that analyze customer preferences and adjust recommendations based on buying patterns (supervised learning).
5. **Network Infrastructure**:
   - **SOHO network proposal**: The e-shop office would require a network setup to handle both internal communications (between employees, databases) and external communications (customer orders, shipping vendors).
   - **Network devices and protocols**: Routers, switches, and firewalls for securing transactions and managing traffic. TCP/IP for data communication.
   - **Client-server model**: Customer requests products (client) and the e-shop server responds with information or processes orders.
6. **Cybersecurity**:
   - **Cybersecurity threats**: Example of an SQL injection attack on the customer database, phishing attacks on users.
   - **CIA triad**: Confidentiality (e.g., encryption of payment details), Integrity (e.g., ensuring that order data isn’t tampered with), and Availability (e.g., ensuring that the website is always online).
   - **Cryptography**: Use of digital signatures for validating payment transactions, and session keys for encrypting communication between the server and the customer.