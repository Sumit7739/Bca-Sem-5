### **1. Introduction to Internet**

- **The Internet**: A global network connecting millions of computers, allowing them to communicate and share information. It uses standard protocols to ensure data is transferred seamlessly between devices worldwide.

### **2. Domains**

- **Domain**: It's the address that you type in a browser's URL bar to access a website (e.g., **[www.example.com](http://www.example.com)**). Domains are human-readable and mapped to IP addresses using a Domain Name System (DNS).
- **Structure of Domain Name**:
    - **Top-Level Domain (TLD)**: The last part of the domain (e.g., **.com**, **.org**, **.in**).
    - **Second-Level Domain**: The unique name chosen by the website owner (e.g., **example** in **[www.example.com](http://www.example.com)**).
    - **Subdomain**: A part of the main domain, like **blog.example.com**.

- **What is a Domain?**  
    A domain is the address people use to access websites on the internet. It's the human-readable version of an IP address.  
    Example: `www.google.com`.
    
- **Parts of a Domain:**
    
    1. **Top-Level Domain (TLD):** The extension at the end of a domain. Examples: `.com`, `.org`, `.edu`.
    2. **Second-Level Domain (SLD):** The name before the TLD. Example: In `google.com`, "google" is the SLD.
    3. **Subdomain:** An optional prefix. Example: `mail.google.com` (subdomain: "mail").
- **Types of Domains:**
    
    - **Generic TLDs (gTLDs):** `.com`, `.net`, `.org`.
    - **Country Code TLDs (ccTLDs):** `.in` (India), `.uk` (United Kingdom).
    - **Virtual Domains:** These represent hosted websites with unique domain names, allowing multiple websites to share a single IP address.

### **3. Virtual Domain**

- **Virtual Domain**: A virtual domain refers to a domain hosted on the same physical server as multiple other websites. It allows different websites to appear as if they have their own individual servers, even though they share one physical machine.
    - **Example**: A web hosting service may host multiple websites using one IP address by assigning each domain a unique virtual host.

- **Definition:**  
    A virtual domain allows multiple domain names to point to the same server or IP address.  
    Example: A hosting service might host both `site1.com` and `site2.com` on the same server.
    
- **How it Works:**
    
    - Virtual domains use server configuration to route traffic based on the domain name requested.
    - Common in shared hosting environments.

### **4. IP Address**

- **IP Address**: A unique number assigned to each device connected to the Internet. It identifies devices in a network.
    - **IPv4**: The most common format, consisting of four sets of numbers (e.g., **192.168.1.1**).
    - **IPv6**: A newer format with a larger address space, written in hexadecimal (e.g., **2001:0db8:85a3:0000:0000:8a2e:0370:7334**).
- **Public vs. Private IP**:
    - **Public IP**: Unique on the global internet, used to identify your device across the internet.
    - **Private IP**: Used within local networks (e.g., at home or in a company) and cannot be reached from outside that network.
- **What is an IP Address?**  
    It’s a unique numerical label assigned to every device connected to a network.  
    Example: `192.168.1.1`.
    
- **Types of IP Addresses:**
    
    1. **IPv4:** Uses a 32-bit number, written as four numbers separated by dots (e.g., `192.0.2.1`).
    2. **IPv6:** Uses a 128-bit number, written as hexadecimal numbers separated by colons (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`).
- **Role:**
    
    - Identifies devices on a network.
    - Helps in routing data packets across the internet.

### **5. TCP/IP and Its Services**

- **TCP/IP (Transmission Control Protocol/Internet Protocol)**: A set of communication protocols that dictate how data is transmitted over the internet. It breaks data into packets, sends them across the network, and ensures they arrive intact.
    - **IP**: Responsible for routing the data packets to the correct destination (addresses the packet).
    - **TCP**: Ensures reliable data transmission by making sure all packets reach their destination and are reassembled correctly.
    - **Other protocols within TCP/IP**:
        - **HTTP/HTTPS**: For browsing websites (Hypertext Transfer Protocol/Secure).
        - **FTP**: For transferring files between computers (File Transfer Protocol).
        - **SMTP**: For sending emails (Simple Mail Transfer Protocol).

- **What is TCP/IP?**  
    Transmission Control Protocol/Internet Protocol is the suite of communication protocols used to connect devices on the internet.
    
- **How TCP/IP Works:**
    
    - **TCP:** Breaks data into packets, ensures delivery, and reassembles them at the destination.
    - **IP:** Handles addressing and routing of packets between sender and receiver.
- **Key Services of TCP/IP:**
    
    1. **File Transfer Protocol (FTP):** Transfers files between systems.
    2. **Simple Mail Transfer Protocol (SMTP):** For sending emails.
    3. **Hypertext Transfer Protocol (HTTP):** For accessing web pages.
    4. **Domain Name System (DNS):** Converts domain names into IP addresses.
### **6. WWW (World Wide Web) & Telnet**

- **WWW (World Wide Web)**: A system of interlinked hypertext documents accessed through the internet. When you browse the internet and access websites, you’re using the [WWW](http://WWW).
    
    - **Web Browser**: Software (like Chrome, Firefox, Safari) used to access and view websites.
    - **Web Page**: A single document on the WWW (e.g., **index.html**).
    - **Web Site**: A collection of web pages and associated resources (images, videos) hosted under a domain name.
- **Telnet**: A network protocol used to provide a command-line interface for communication with remote computers. It allows users to log into other computers over the internet and manage files or settings.
    
    - **Security Concern**: Telnet is not secure because data, including passwords, is transmitted in plain text. **SSH (Secure Shell)** is often used as a secure alternative.

- **What is the WWW?**  
    The WWW is a collection of web pages and resources interconnected by hyperlinks and accessed via the internet using web browsers.
    
- **Components of the WWW:**
    
    1. **Web Pages:** Documents written in HTML.
    2. **Hyperlinks:** Links that connect web pages.
    3. **Web Browsers:** Software like Chrome, Firefox, or Safari used to access the [WWW](http://WWW).
- **How it Works:**
    
    - A browser sends an HTTP request to a web server.
    - The server responds with the requested web page.
### **7. Web Server**

- **Web Server**: A computer or software that stores websites and serves web pages to users over the internet. When you request a website, the web server sends the requested page to your browser.
    - **Popular Web Servers**:
        - **Apache HTTP Server**: Open-source, widely used.
        - **Nginx**: A high-performance web server used for large traffic.
    - **Functions of a Web Server**:
        - **Host Websites**: Store files like HTML, CSS, JavaScript, images, etc.
        - **Respond to Requests**: Send requested web pages to users when they visit a website.
        - **Handle Requests via HTTP/HTTPS**: Manage and serve data based on the user’s requests.
        - **Support Scripts**: Can execute server-side scripts (e.g., PHP, Python).

-  **What is a Web Server?**  
    A web server is software or hardware that serves web pages to users in response to their HTTP requests.
    
- **Examples of Web Servers:**
    
    1. **Apache HTTP Server:** Open-source, highly customizable.
    2. **Nginx:** Known for its speed and scalability.
    3. **Microsoft IIS:** Integrated with Windows Server.
- **Functions of a Web Server:**
    
    1. Stores and serves web pages.
    2. Handles user requests and sends responses.
    3. Manages resources like databases and scripts.

### 8. What is Telnet?  
    
Telnet is a protocol that allows users to remotely access and manage devices over a network.
    
- **Features:**
    
    - Provides a command-line interface for communication with a remote computer.
    - Useful for network administrators.
- **Limitations:**
    
    - No encryption, making it insecure.
    - Replaced by more secure protocols like SSH (Secure Shell).
---

### Quick Summary:

- **Domains** make websites accessible by human-readable names.
- **Virtual Domains** allow hosting multiple sites on the same server.
- **IP Addresses** identify devices on the internet, ensuring they can be reached.
- **TCP/IP** is the protocol suite that allows communication and ensures reliable data delivery.
- **WWW** is the collection of websites you interact with, and **Telnet** is an old command-line interface for remote control of systems.
- **Web Servers** store websites and send web pages when users request them.

---

<!-- Next ->  [[Sgml and Html]] -->
[Next](SgmlandHtml.md)