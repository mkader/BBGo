Static Algorithms
1. Round robin - The client requests are sent to different service instances in sequential order. The services are usually required to be stateless.

2. Sticky round-robin - This is an improvement of the round-robin algorithm. If Alice’s first request goes to service A, the following requests go to service A as well.

3. Weighted round-robin - The admin can specify the weight for each service. The ones with a higher weight handle more requests than others.

4. Hash - This algorithm applies a hash function on the incoming requests’ IP or URL. The requests are routed to relevant instances based on the hash function result.

Dynamic Algorithms
5. Least connections - A new request is sent to the service instance with the least concurrent connections.

6. Least response time - A new request is sent to the service instance with the fastest response time.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/a8107d0d-57fb-4f5d-810a-561c09494c49_1604x1536.jpeg">
