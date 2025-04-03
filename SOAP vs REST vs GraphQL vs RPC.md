<img src="https://substack-post-media.s3.amazonaws.com/public/images/972d1d02-396b-4464-b8a3-320b0cbd0f6f_1743x1536.jpeg">

## REST API Vs. GraphQL

* REST
  1. Uses standard HTTP methods like GET, POST, PUT, DELETE for CRUD operations.
  1. Works well when you need simple, uniform interfaces between separate services/applications.
  1. Caching strategies are straightforward to implement.
  1. The downside is it may require multiple roundtrips to assemble related data from separate endpoints.

* GraphQL
  1. Provides a single endpoint for clients to query for precisely the data they need.
  1. Clients specify the exact fields required in nested queries, and the server returns optimized payloads containing just those fields.
  1. Supports Mutations for modifying data and Subscriptions for real-time notifications.
  1. Great for aggregating data from multiple sources and works well with rapidly evolving frontend requirements.
  1. However, it shifts complexity to the client side and can allow abusive queries if not properly safeguarded
  1. Caching strategies can be more complicated than REST.

* The best choice between REST and GraphQL depends on the specific requirements of the application and development team. GraphQL is a good fit for complex or frequently changing frontend needs, while REST suits applications where simple and consistent contracts are preferred.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/a2a0d504-996d-4790-aaa3-ae39e1eee5f6_1280x1663.gif">

* gRPC work
  1. RPC (Remote Procedure Call) is called “remote” because it enables communications between remote services when services are deployed to different servers under microservice architecture. From the user’s point of view, it acts like a local function call.
  1. The diagram below illustrates the overall data flow for gRPC.
    * Step 1: A REST call is made from the client. The request body is usually in JSON format.
    * Steps 2 - 4: The order service (gRPC client) receives the REST call, transforms it, and makes an RPC call to the payment service. gPRC encodes the client stub into a binary format and sends it to the low-level transport layer.
    * Step 5: gRPC sends the packets over the network via HTTP2. Because of binary encoding and network optimizations, gRPC is said to be 5X faster than JSON.
    * Steps 6 - 8: The payment service (gRPC server) receives the packets from the network, decodes them, and invokes the server application.
    * Steps 9 - 11: The result is returned from the server application, and gets encoded and sent to the transport layer.
    * Steps 12 - 14: The order service receives the packets, decodes them, and sends the result to the client application.
<img src="https://substack-post-media.s3.amazonaws.com/public/images/52fabbbd-7ac2-4913-a696-3dc9fe625a91_1280x1664.gif">
