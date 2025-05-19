# Rate Limiting

##  Definition
Rate limiting is a technique used to control how many requests a user or system can make in a given time period. 
It helps prevent abuse, reduce server overload, and ensure fair usage of resources.
![image](https://github.com/user-attachments/assets/example-rate-limiting-diagram)

##  Why It’s Important
Without rate limiting, a user or bot could send thousands of requests per second, which could slow down or crash your system. 
Rate limiting protects your services by rejecting or delaying extra requests that exceed a safe limit.

## How It Works
Each user or IP address is tracked with a counter. If the number of requests in a time window (like per second or minute) 
exceeds the limit, the system blocks or delays further requests. Common algorithms include token bucket, leaky bucket, and 
fixed window counters.

##  Real-world Examples
APIs like Twitter, GitHub, and Google Maps use rate limiting to prevent users from overusing their services. 
For example, the GitHub API might only allow 60 requests per minute for unauthenticated users.

##  Trade-offs
Rate limiting adds some complexity, especially when implemented in distributed systems. 
It can also block legitimate users during peak traffic times if the limits are too strict. 
Choosing the right limits is important for balancing performance and fairness.

##  When to Use / When Not To
Use rate limiting when exposing APIs, login systems, or any service that might be abused or receive unpredictable traffic. 
Avoid using it in internal-only systems with full trust unless there's a risk of accidental overload.

##  Further Reading
https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Retry-After  
https://cloudflare.com/learning/ddos/glossary/rate-limiting/  
https://stripe.com/blog/rate-limiters
