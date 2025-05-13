 Caching

##  Definition
Caching is a technique used to store copies of frequently used data in a temporary storage area. 
This allows systems to quickly serve future requests for the same data without needing to fetch it again from the original source.
![image](https://github.com/user-attachments/assets/e72b7bdf-794f-4795-8915-326bcacfd68f)


##  Why It’s Important
Every time a user visits a page or requests information, the system might have to access a database or perform a complex calculation. 
This takes time. Caching speeds things up by serving the saved version of the data, reducing delay and saving server resources.

## How It Works
When a user makes a request, the system first checks if a cached version of the data is available. 
If it is, that version is returned immediately. If not, the system fetches fresh data from the source, saves it in the cache, and then returns it. 
Caches can be stored in memory (RAM), on disk, or even in browsers.

##  Real-world Examples
Google Chrome uses browser caching to save website data locally so it doesn’t have to reload images or styles every time. 
YouTube uses caching to store popular videos on nearby servers (using CDNs), so users get faster streaming without buffering.

##  Trade-offs
Caching improves speed and reduces load on servers, but the main problem is data freshness. 
If the original data changes but the cache is not updated, users may see outdated information. 
This is known as a “stale cache.” Also, too much caching can use a lot of memory.

##  When to Use / When Not To
Caching is useful when your application frequently serves the same data, like product details or blog pages. 
However, avoid caching when the data changes very frequently or needs to be 100% real-time, like live stock prices or transaction-data.

##  Further Reading
- [How Caching Works (MDN)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching)
- [Caching Strategies by Cloudflare](https://www.cloudflare.com/learning/cdn/what-is-caching/)
- [YouTube: What is Caching? (Tech with Tim)](https://www.youtube.com/watch?v=RZ4p-saaQkc)
