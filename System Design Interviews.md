* Follow this 7-step process to do well in a System Design Round
  1. Requirements Clarification: In the first step, clarify functional and non-functional requirements. Ask questions to understand the core features of the system as well as non-functional aspects such as data volume, availability, scale, etc.
  2. Capacity Estimation: Next, estimate the capacity of the system. Focus on attributes like the number of users, traffic, storage/memory needs, and compute and networking requirements.
  3. Create High-Level Design: Break down the system into components such as client apps, servers, load balancers, databases, etc. Start with drawing a simple block diagram that shows these components and their potential interaction with each other. Focus on the data flow.
  4. Database Design: Model the data and choose the right database type for the system. Once done, focus on the database schema.
  5. Interface Design: Next, focus on the interfaces to the system. This could be API endpoints or event models exchanged between the various components of the system. Also, choose a communication approach such as REST, GraphQL, gRPC, or an event-driven
  6. Scalability and Performance: Address the scalability, performance, and latency aspects of the system by suggesting techniques that will be used. For example, vertical and horizontal scaling, caching, indexing, denormalizing, sharding, replication, CDNs, etc.
  7. Reliability and Resiliency: Lastly, address the reliability and resiliency of the design. Identify single points of failure and mitigate their impact.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/e038f714-2624-4191-9531-77df101aa2e1_1280x1657.gif">

* They are the most critical components to crafting successful software systems.
* Let’s look at each of them with implementation techniques:
  1. Scalability: Scalability ensures that your application can handle more load without compromising performance.
  1. Availability: Availability makes sure that your application is always ready to serve the users and downtime is minimal.
  1. Reliability: Reliability is about building software that consistently delivers correct results.
  1. Performance: Performance is the ability of a system to carry out its tasks at an expected rate under peak load using available resources.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/77498aa3-aa02-4a5f-ac0a-3db855f5122b_1286x1536.gif">
