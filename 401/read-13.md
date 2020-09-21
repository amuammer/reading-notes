# JWT

### What is JSON Web Token?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.


### What is the JSON Web Token structure?

In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are: <br/>
**Header** <br/>
**Payload** <br/>
**Signature** <br/>

<img src="https://cdn.auth0.com/blog/legacy-app-auth/legacy-app-auth-5.png" />

### Token-based authentication

**Token-based authentication** is one in which the user state is stored on the client. This has grown to be the preferred mode of authentication for RESTful APIs. In the token-based authentication, the user data is encrypted into a JWT (JSON Web Token) with a secret and then sent back to the client. <br/>
The JWT is then stored on the client-side mostly localStorage and sent as a header for every subsequent request. The server receives and validates the JWT before proceeding to send a response to the client.

```javascript
headers:{
"Authorization": "Bearer ${JWT_TOKEN}"
}
```

<img src="https://miro.medium.com/max/679/0*asCYoVfW9O5cmRHt.png" />
