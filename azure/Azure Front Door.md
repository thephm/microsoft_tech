# Azure Front Door

Azure Front Door is a scalable and secure entry point for web applications, providing global HTTP load balancing and site acceleration. It is designed to offer developers and administrators a way to deliver content and services at high throughput and low latency by routing and distributing web traffic across the global Microsoft network. Here are the key features and functionalities of Azure Front Door:​

- Global HTTP Load Balancing: Azure Front Door uses the Microsoft global network to distribute HTTP/HTTPS traffic to the closest available point-of-presence (PoP) location. This helps in reducing latency by serving requests from geographical locations closest to the users.​
    
- SSL Offloading and Application Acceleration: It handles SSL/TLS termination at the edge close to the user, which reduces the load on your web servers and accelerates application performance. This is particularly beneficial for optimizing content delivery and improving user experience.​
    
- URL-Based Routing: Requests can be routed based on URL path or other parameters. This allows different paths within your application to be handled by different pools of resources, providing flexibility and efficient use of resources.​
    
- Session Affinity: Azure Front Door supports session affinity, which is crucial for ensuring that all requests from a particular user session are sent to the same backend during a session. This is important for applications that maintain user state on a specific server.​
    
- Instant Global Failover: Provides the ability to failover traffic to different backends in real-time. This is essential for high availability and resilience, ensuring that user requests can always be served even if a backend goes down.​
    
- Integrated Web Application Firewall (WAF): Azure Front Door comes with a built-in Web Application Firewall that helps protect your applications from common exploits and vulnerabilities. WAF rules can be customized to meet the specific security needs of your applications.​
    
- Caching: Content can be cached at edge locations around the world, which reduces load times, decreases load on the web servers, and improves overall application responsiveness.​
    
- Health Probes: Azure Front Door automatically performs health checks on your backends to ensure traffic is only sent to healthy instances. This increases the reliability of your applications by avoiding servers that are down or not responding.​
    
- Custom Routing Rules: Supports creating custom routing rules based on the application’s needs, such as redirecting traffic under certain conditions, rewriting URLs, or even stripping headers before forwarding requests to the backend.​
    
- Secure and Compliant: Complies with key compliance standards, providing a secure environment for handling data and transactions.​