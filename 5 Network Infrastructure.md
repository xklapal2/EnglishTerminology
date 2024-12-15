### **Network Infrastructure**

A robust network infrastructure is essential for the seamless operation of an e-shop, ensuring reliable communication between internal systems and external stakeholders such as customers and vendors.

---

### **1. SOHO Network Proposal**

For a **Small Office/Home Office (SOHO)** setup, the e-shop’s network must support both internal and external communications:

1. **Internal Communications**:
    
    - Employees accessing the database for inventory management.
    - Secure communication between departments (e.g., sales, support, shipping).
2. **External Communications**:
    
    - Handling customer orders from the website.
    - Communicating with shipping vendors for delivery updates.

A typical network setup would include a local area network (LAN) for internal communication and a connection to the internet for external communication.

---

### **2. Network Devices and Protocols**

To support the e-shop’s operations, several network devices and protocols are required:

#### **a) Network Devices**

- **Router**:
    
    - Connects the office LAN to the internet.
    - Provides NAT (Network Address Translation) for secure access.
    - Handles external requests, such as processing orders or communicating with customers.
- **Switch**:
    
    - Facilitates communication within the office network by connecting devices such as computers, printers, and servers.
    - Ensures efficient data transfer between endpoints.
- **Firewall**:
    
    - Protects the network from unauthorized access and cyber threats.
    - Filters incoming and outgoing traffic to secure sensitive data like customer information and payment details.
- **Access Point (optional)**:
    
    - Provides Wi-Fi connectivity for employee devices within the office.

#### **b) Protocols**

- **TCP/IP**:
    
    - The foundational protocol suite for internet communication.
    - Ensures reliable data transfer between the e-shop’s server and customer devices.
- **HTTP/HTTPS**:
    
    - HTTP facilitates web communication, while HTTPS secures it using encryption for transactions and sensitive information.
    - Essential for the e-shop website to protect customer data.
- **FTP/SFTP**:
    
    - For transferring large files, such as product images or bulk inventory updates, between systems.
- **DNS**:
    
    - Converts domain names (e.g., [www.eshop.com](http://www.eshop.com)) into IP addresses to route traffic correctly.

---

### **3. Client-Server Model**

The e-shop operates on a **client-server architecture**, a common model in networked applications:

- **Client**:
    
    - Represents the customer’s device (e.g., browser or mobile app).
    - Sends requests to the server, such as searching for a product or placing an order.
- **Server**:
    
    - Responds to client requests by delivering information (e.g., product details) or executing actions (e.g., processing orders).
    - Maintains the database of products, customer profiles, and order histories.

#### **Example Workflow**:

1. A customer searches for a product on the website.
2. The client (browser) sends a request to the server via HTTP.
3. The server queries the database for matching products.
4. Results are sent back to the client, and the page is updated with the search results.

---

### **4. Benefits of a Well-Designed Network**

1. **Efficiency**: Ensures fast and reliable communication between internal systems and external users.
2. **Scalability**: Allows for easy expansion as the business grows (e.g., adding more devices or locations).
3. **Security**: Protects sensitive data with firewalls, encryption, and secure protocols.
4. **Business Continuity**: Reduces downtime by using reliable network equipment and redundant connections.

---

### **Conclusion**

A strong network infrastructure is the backbone of the e-shop, enabling seamless internal operations and smooth customer interactions. By using appropriate devices, protocols, and a client-server model, the e-shop ensures secure and efficient communication at all times.