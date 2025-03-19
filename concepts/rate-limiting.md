# Rate Limiting 

Why Rate Limiting is important in Scalable Systems ?
Every system has a breaking point — and without control, even the best APIs and services can fail under heavy load.

That is where Rate Limiting comes in — a mechanism to protect your services, ensure fair usage, and maintain high availability.

💡 But how does Rate Limiting work under the hood?

Let me introduce you to one of the most popular algorithms:

 🎯 The Token Bucket Algorithm:

👉 Imagine a bucket that holds tokens (each token represents permission to process 1 request).
 👉 The bucket refills tokens at a fixed rate (e.g., 5 tokens/sec).
 👉 When a request comes in, it takes a token from the bucket:

✅ If a token is available, the request is allowed.
❌ If the bucket is empty (no tokens left), the request is denied or delayed.

✨ Why is Token Bucket powerful?
Handles bursts gracefully (if tokens are available, it allows quick bursts).
Smooths traffic over time (avoids overwhelming backend services).
Flexible control over how fast and how much traffic is allowed.

✅ Takeaway:
 If you're building or working with APIs, rate limiting isn't optional — it's a shield that protects your system and your users.



https://github.com/user-attachments/assets/4e04755b-0413-4598-9945-3240b2485be4

