* Both tokens (such as JWT) and API keys are used for authentication and authorization, but they serve different purposes. Let’s understand the simplified flow for both.

## The Token Flow
1. End user logs into the frontend web application.
1. Login credentials are sent to the Identity Service.
1. On successful authentication, a JWT token is issued and returned.
1. The frontend makes API calls with the JWT in the Authorization header.
1. API Gateway intercepts the request and validates the JWT (signature, expiry, and claims).
1. If valid, the gateway sends a validation response.
1. The validated request is forwarded to the user-authenticated service.
1. The service processes the request and interacts with the database to return results.

## The API Key Flow
1. A 3rd party developer registers on the Developer Portal.
1. The portal issues an API Key.
1. The key is also stored in a secure key store for later verification.
1. The developer app sends future API requests with the API Key in the header.
1. The API Gateway intercepts the request and sends the key to the API Key Validation service.
1. The validation service verifies the key from the key store and responds.
1. For valid API keys, the gateway forwards the request to the public API service.
1. The service processes it and accesses the database as needed.

<img src="https://github.com/mkader/BBGo/blob/b0be89a19f6ba3ad8aa350783bd28c4b78a917e7/Tokens%20vs%20API%20Keys.jpg"/>
