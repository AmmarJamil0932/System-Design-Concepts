# Load Balancing

##  Definition
Load balancing is a method used to share incoming traffic evenly across multiple servers. 
This means that no single server is doing all the work, which helps the system run more smoothly and quickly.
![image](https://github.com/user-attachments/assets/67f4733f-8c3c-4bfe-9200-93e43cf6aaca)

##  Why It’s Important
In large systems, thousands or even millions of users can send requests at the same time. 
If one server handles all the requests, it can get slow or crash. Load balancing helps by 
spreading the traffic to multiple servers so everything works faster and stays online.

## How It Works
A load balancer sits between users and the servers. When a user sends a request, 
the load balancer chooses one of the servers to handle it. It can do this using different
methods like Round Robin (taking turns), Least Connections (choosing the server with the fewest
users), or based on server speed or location. This helps balance the load smartly.

##  Real-world Examples
Big companies like Amazon, Google, and Netflix use load balancers to manage their traffic. 
For example, when you visit Amazon’s website, a load balancer sends your request to the neares
t or least busy server so your page loads quickly.

##  Trade-offs
While load balancing helps improve performance and uptime, it also adds extra setup. 
If the load balancer itself fails and there is no backup, the whole system can stop working. 
Also, sometimes it might choose a slower server by mistake if the logic isn’t set up properly.

##  When to Use / When Not To
You should use load balancing if your website or app has many users and needs to stay available all the time. 
It’s also useful when your system has multiple servers doing the same job. However, if you're building a small 
personal project with only one server, load balancing might be unnecessary and too complex.

##  Further Reading
- [AWS Load Balancer Documentation](https://docs.aws.amazon.com/elasticloadbalancing/)
- [NGINX Load Balancing Guide](https://www.nginx.com/resources/glossary/load-balancing/)
- [YouTube: Load Balancer Explained Simply](https://www.youtube.com/watch?v=4PzI6yFf8So)
