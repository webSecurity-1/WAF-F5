# Web Application Firewall "F5"

<img src="https://www.cloudflare.com/img/learning/ddos/glossary/waf/waf.png" />

## Web Application Firewalls (WAF)

<p align="justify">Is a security solution specifically designed to protect web applications from various types of attacks, such as cross-site scripting (XSS), SQL injection, and application-layer DDoS attacks. It focuses on the <b>application layer</b> of the network stack and is typically deployed in front of web servers to filter and monitor incoming and outgoing HTTP/HTTPS traffic
</p>

<hr>

## Types of WAF

There are three primary ways to implement a WAF:

- Network-based (NWAF): Traditionally hardware-based in an on-premises environment.

- Host-based: WAF is implemented as an additional application or plugin on a web server.

- Cloud-based: WAF protection is transferred to an external cloud supplier.

<hr>

## WAF Detection Methods

<p align="justify">
A Web Application Firewall (WAF) detects abnormal behavior by analyzing the incoming traffic to a web application and comparing it against predefined security rules and patterns. Here are some common methods used by WAFs to detect abnormal behavior:
</p>

- Signature-based detection

- Regex-based detection

- Challenge/Response detection (virusTotal)

- Abnormal Behaviors detection

<p align="justify">
It's important to note that WAFs use a combination of these methods to provide comprehensive protection. The specific techniques and algorithms employed may vary depending on the WAF vendor and its capabilities.
</p>

<hr>

> ## Let's Start with F5


## What is F5?

<p align="justify">
F5 Networks is a company that specializes in providing various networking and security solutions, including load balancing, application delivery controllers, and security services. One of their flagship products is the TMOS (Traffic Management Operating System), which powers F5's BIG-IP platform.
</p>

<hr />

## F5 Full Proxy Architecture

<img src="https://i.ibb.co/vPWM3nM/1.png" alt="1" border="0">

<hr />

## Anatomy of Web Application 

<p align="justify">
In the past, websites were primarily static, meaning that their content remained fixed and unchanged until manually updated by the website owner. These static websites consisted of HTML files that were stored on a server and served to users' web browsers upon request. While static websites served their purpose of providing information, they lacked interactivity and dynamic functionality.

As the web evolved, the concept of web applications emerged. Web applications are dynamic websites that allow users to interact with the content and perform various tasks. They introduced a more sophisticated architecture and utilized different technologies to provide a richer user experience.

The anatomy of a web application consists of several key components that work together to deliver the desired functionality:

- <b>Front-end:</b> The front-end encompasses the client-side components responsible for the visual presentation and user interaction. It typically involves HTML for structure, CSS for styling, and JavaScript for dynamic behavior. Modern front-end frameworks like React, Angular, or Vue.js simplify the development process and offer advanced capabilities.

- <b>Back-end:</b> The back-end comprises the server-side components that handle the business logic and data processing. It involves programming languages such as Python, JavaScript (Node.js), Ruby, or Java, along with frameworks like Django, Flask, Express.js, Ruby on Rails, or Spring.


- <b>Database:</b> Web applications often require persistent data storage. Databases such as MySQL, PostgreSQL, MongoDB, or Redis are commonly used to store and retrieve data on the server-side. They enable efficient data management and provide structured access to information.


Over time, the anatomy of web applications has evolved significantly, driven by advancements in technology, frameworks, and development practices. The shift from static websites to dynamic web applications has revolutionized the way we interact with online content, enabling sophisticated features, real-time updates, and personalized experiences.
</p>


<img src="https://i.ibb.co/p2zJ2wR/1.jpg" alt="1" border="0">


<hr />

### SQL injection and cross site scripting remain the most critical web vulnerabilities

> ## So Let's go with BIG-IP ASM


<hr />

## BIG-IP ASM

<p align="justify">
BIG-IP ASM stands for BIG-IP Application Security Manager. It is a module or component of the F5 Networks' BIG-IP product suite, which provides advanced application security and protection against a wide range of attacks. BIG-IP ASM is designed to safeguard web applications from vulnerabilities, such as SQL injection, cross-site scripting (XSS), and remote file inclusion, among others.
</p>

## Using BIG-IP ASM to protect web applications

- Buffer Overflow
- OWASP top ten
- Layer 7 DDOS
- Botnet Detection
- Geolocation enforcement

<hr />

## BIG-IP ASM Features

<p align="justify">
BIG-IP ASM provides a wide range of features to protect web applications from various types of attacks and vulnerabilities. Here are some of the key features of BIG-IP ASM:

- <b>Web Application Firewall (WAF)</b>: BIG-IP ASM provides a comprehensive WAF solution to protect web applications from various types of attacks, such as SQL injection, cross-site scripting (XSS), and remote file inclusion, among others.

- <b>Application Layer DDoS Protection</b>: BIG-IP ASM provides application layer DDoS protection to protect web applications from DDoS attacks, such as HTTP floods, slow HTTP post attacks, and DNS amplification attacks, among others.

- <b>Bot Protection</b>: BIG-IP ASM provides bot protection to protect web applications from malicious bots, such as web scrapers, content scrapers, and vulnerability scanners, among others.

- <b>SSL/TLS Offloading</b>: BIG-IP ASM provides SSL/TLS offloading to offload SSL/TLS processing from web servers to BIG-IP ASM, which helps improve performance and scalability.

- <b>Geolocation Enforcement</b>: BIG-IP ASM provides geolocation enforcement to restrict access to web applications based on the user's location.
<hr >

## Why ASM

- It Examine an Http Request.
- It can check for various length limit.
- It can Enforce Specific File Type.
- It can check each parameters for specific criteria.
- It can verify the Server Response.

<hr />

## ASM vs Traditional Security Devices

<img src="https://i.ibb.co/0Zgtnpt/compare.webp" alt="compare" border="0">

<hr />

## Types of Computer Security

<img src="https://i.ibb.co/K6tLDF1/black-white-lists.png" alt="black-white-lists" border="0">

<hr />

## ASM Policy Building

 A security policy is a set of rules that define how BIG-IP ASM should protect a web application. It consists of security checks, which are used to detect and prevent attacks against the web application. BIG-IP ASM provides a wide range of security checks to protect web applications from various types of attacks, such as SQL injection, cross-site scripting (XSS), and remote file inclusion, among others.


- <b>Learning Settings</b>: Learning settings define how BIG-IP ASM should learn the web application. BIG-IP ASM provides a wide range of learning settings to learn the web application, such as learning the parameters, learning the URLs, or learning the cookies, among others.

- <b>Blocking Settings</b>: Blocking settings define how BIG-IP ASM should block malicious requests. BIG-IP ASM provides a wide range of blocking settings to block malicious requests, such as blocking the request, blocking the session, or blocking the IP address, among others.

- <b>Whitelist Settings</b>: Whitelist settings define how BIG-IP ASM should whitelist certain requests. BIG-IP ASM provides a wide range of whitelist settings to whitelist certain requests, such as whitelisting the IP address, whitelisting the URL, or whitelisting the parameter, among others.


- <b>Reporting Settings</b>: Reporting settings define how BIG-IP ASM should report security events. BIG-IP ASM provides a wide range of reporting settings to report security events, such as sending an email notification, sending an SNMP trap, or logging the event, among others.

<hr />

<p align="justify">
Overall, BIG-IP ASM is a powerful solution for securing web applications, providing comprehensive protection against various types of attacks and vulnerabilities. It helps organizations ensure the availability, integrity, and confidentiality of their critical web applications and protect sensitive data from unauthorized access or compromise.
</p>
