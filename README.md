# Web Application Firewall "F5"

<img src="https://www.cloudflare.com/img/learning/ddos/glossary/waf/waf.png" />

## Web Application Firewalls (WAF)

<p align="justify">Is a security solution specifically designed to protect web applications from various types of attacks, such as cross-site scripting (XSS), SQL injection, and application-layer DDoS attacks. It focuses on the <b>application layer</b> of the network stack and is typically deployed in front of web servers to filter and monitor incoming and outgoing HTTP/HTTPS traffic
</p>

<hr>

## Types of Web Application Firewalls

There are three primary ways to implement a WAF:

- Network-based (NWAF): Traditionally hardware-based in an on-premises environment.

- Host-based: WAF is implemented as an additional application or plugin on a web server.

- Cloud-based: WAF protection is transferred to an external cloud supplier.

<hr>

<!-- ## How does a WAF work?

A WAF is usually placed logically between users and web servers and analyzes and compares network traffic with the vulnerability database. A WAF creates a set of rules designed to protect your website and detects unwanted traffic. It usually blocks this traffic but can be set up to only monitor it. -->

## WAF Detection Methods
<p align="justify">
A Web Application Firewall (WAF) detects abnormal behavior by analyzing the incoming traffic to a web application and comparing it against predefined security rules and patterns. Here are some common methods used by WAFs to detect abnormal behavior:

- Signature-based detection: WAFs maintain a database of known attack signatures, such as patterns in URLs, request parameters, or payloads associated with common attacks like SQL injection or cross-site scripting (XSS). If the incoming traffic matches any of these signatures, the WAF identifies it as potentially malicious.

- Anomaly-based detection: WAFs establish a baseline of normal behavior by analyzing legitimate traffic patterns and request characteristics. They monitor incoming requests for deviations from this baseline. If a request significantly deviates from expected behavior, it may be flagged as suspicious or potentially malicious. Examples of anomalies include an unusually high request rate, abnormally large requests, or unexpected sequence of requests.

- Behavioral analysis: Some advanced WAFs employ machine learning and behavioral analysis techniques to identify abnormal behavior. They build models by analyzing historical traffic patterns and use them to detect deviations from the expected behavior. By continuously learning and adapting to new traffic patterns, these WAFs can detect emerging threats and zero-day attacks.

- Protocol and semantic analysis: WAFs inspect the structure and semantics of web application protocols, such as HTTP, to detect anomalies. They analyze the HTTP headers, cookies, and payloads for inconsistencies, malformed requests, or suspicious content. For example, a WAF might look for unexpected HTTP methods, excessive parameter manipulation, or attempts to bypass security controls.

- Reputation-based detection: WAFs may leverage reputation services or threat intelligence feeds to identify known malicious IP addresses, domains, or user agents. If an incoming request originates from a blacklisted source, the WAF can block or flag it as suspicious.

It's important to note that WAFs use a combination of these methods to provide comprehensive protection. The specific techniques and algorithms employed may vary depending on the WAF vendor and its capabilities.
</p>