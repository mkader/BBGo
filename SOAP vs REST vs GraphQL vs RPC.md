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
