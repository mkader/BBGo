1. Step 1 - The client sends an HTTP request to the API gateway.
1. Step 2 - The API gateway parses and validates the attributes in the HTTP request.
1. Step 3 - The API gateway performs allow-list/deny-list checks.
1. Step 4 - The API gateway talks to an identity provider for authentication and authorization.
1. Step 5 - The rate limiting rules are applied to the request. If it is over the limit, the request is rejected.
1. Steps 6 and 7 - Now that the request has passed basic checks, the API gateway finds the relevant service to route to by path matching.
1. Step 8 - The API gateway transforms the request into the appropriate protocol and sends it to backend microservices.
1. Steps 9-12: The API gateway can handle errors properly, and deals with faults if the error takes a longer time to recover (circuit break). It can also leverage ELK (Elastic-Logstash-Kibana) stack for logging and monitoring. We sometimes cache data in the API gateway.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/924c1e3f-dcea-4894-8c00-cc87b86f3c16_1280x1664.gif">
