JWTs
  JWT or JSON Web Tokens is an open standard for securely transmitting information between two parties.
  A JWT consists of a Header, Payload, and Signature.
  JWTs can be used to implement stateless authentication between client and server applications.


PASETO ( Platform-Agnostic Security Tokens)
  PASETO is a modern alternative to JWT. It addresses JWT's security flaws by implementing secure defaults.
  Unlike JWT, PASETO enforces strong, cryptographically sound algorithms, reducing the risk of vulnerabilities.
  A PASETO typically consists of Version, Purpose, and Payload. There are two types of PASETO:
  Public PASETO: They are signed using asymmetric cryptography and ensure the integrity of the data, but not its confidentiality.
  Local PASETO: They are encrypted using symmetric encryption algorithms, ensuring the confidentiality of the data contained within the token.

<img src="https://github.com/mkader/BBGo/blob/19984126389a0a2122c316fdd01f1b9b7a85b4f8/JWT%20vs%20PASETO.jpg">
