### **Cybersecurity**

Cybersecurity is a critical aspect of managing an e-shop, protecting sensitive customer data, ensuring the integrity of operations, and maintaining the trust of users.

---

### **1. Cybersecurity Threats**

E-shops face a variety of threats that could compromise their operations and reputation:

#### **a) SQL Injection Attacks**

- **Description**:
    - Attackers exploit vulnerabilities in the website's input fields (e.g., login or search forms) to execute malicious SQL commands on the database.
- **Impact**:
    - Exposure of sensitive customer information such as email addresses, payment details, and order histories.
    - Unauthorized access to the database.

#### **b) Phishing Attacks**

- **Description**:
    - Attackers send fake emails or messages to customers, impersonating the e-shop, to steal sensitive information like passwords or credit card numbers.
- **Impact**:
    - Loss of customer trust and possible financial damages to both customers and the business.

---

### **2. CIA Triad**

The **CIA triad** (Confidentiality, Integrity, Availability) is the foundation of effective cybersecurity measures:

#### **a) Confidentiality**

- Ensuring that sensitive data, such as customer payment details and personal information, is accessible only to authorized parties.
- **Example**:
    - Encrypting payment details during transactions using SSL/TLS.

#### **b) Integrity**

- Protecting data from unauthorized modifications to ensure accuracy and reliability.
- **Example**:
    - Implementing checksums or hash functions to verify that order data has not been tampered with during processing.

#### **c) Availability**

- Ensuring that the e-shop's website and services remain operational and accessible to users.
- **Example**:
    - Using redundant servers and load balancing to handle high traffic or mitigate DDoS attacks.

---

### **3. Cryptography**

Cryptographic techniques play a vital role in securing communications and transactions:

#### **a) Digital Signatures**

- **Use**:
    - Verifying the authenticity and integrity of payment transactions.
    - Ensures that data sent by the payment gateway or customer has not been altered.
- **How It Works**:
    - The e-shop or payment processor signs a transaction with its private key.
    - Customers or banks verify the signature using the corresponding public key.

#### **b) Session Keys**

- **Use**:
    - Encrypting communication between the e-shop’s server and customer devices during a browsing session.
- **How It Works**:
    - A session key is generated for each user session and used for encrypting data exchanges, ensuring confidentiality.
    - Session keys are typically established using algorithms like Diffie-Hellman or RSA.

#### **c) SSL/TLS Protocols**

- Ensures secure communication by encrypting data transmitted between the customer and the server.
- Prevents eavesdropping and man-in-the-middle attacks during checkout or data submission.

---

### **4. Strategies for Enhanced Cybersecurity**

1. **Regular Vulnerability Assessments**:
    
    - Identify and fix security flaws in the website, particularly input fields vulnerable to SQL injections.
2. **Employee Training**:
    
    - Educate employees on recognizing phishing attempts and following best practices for data handling.
3. **Two-Factor Authentication (2FA)**:
    
    - Require customers and employees to verify their identity using a second factor, such as a text message or an authentication app.
4. **Secure Backup Systems**:
    
    - Regularly back up customer and order data to mitigate the impact of ransomware attacks or server failures.
5. **Incident Response Plan**:
    
    - Develop a comprehensive plan to handle data breaches, minimizing downtime and potential damage.

---

### **Conclusion**

By addressing threats such as SQL injections and phishing, adhering to the CIA triad principles, and leveraging cryptographic methods like digital signatures and session keys, the e-shop can create a secure environment for both customers and internal operations. Proactive cybersecurity measures ensure the business’s reputation and functionality are safeguarded against potential threats.