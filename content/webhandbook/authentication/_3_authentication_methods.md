---
title: 3. Authentication methods on the web
description : "Authentication methods on the web"
tags: ["authentication", "authentication methods"]
---

After an authentication type has been chosen, the next step is to determine what method of authentication on the web will be used. A website client is in constant communication with the webserver, sending a request each time a resource is needed. Each of those request needs a proof of authentication to make sure sensitive data cannot be accessed by unauthorized user. Instead of making the user authenticate themselves for each request to the server, there are different ways to store and communicate the credentials safely with the server.

In the following parts different authentication methods and their workflow are explained on a general level without going into specific implementation details. Pros and cons of each method are stated to give an idea of when these methods are useful and what security concerns to look out for.

### 3.1 HTTP Basic Authentication and Digest
Authentication is built into the HTTP Protocol and one of the simplest authentication methods. The server returns a 401 Unauthorized together with a www-Authenticate header telling the client what kind of authentication is required. The options are HTTP Basic or HTTP Digest.

__HTTP Basic__
The username and password are concatenated and encoded with Base64. The encoded string is then sent together with the Authorization header to the server. The server compares the credentials with the database and return a 200 OK if the credentials are valid.

This method is fast, easy to implement and supported in all browser. However, the password and username are only encoded and not encrypted in this method, thus making it vulnerable to attacks that could capture the user’s credentials in transit. It should not be used anymore due to its weak security but is still employed more often than it should be.

__HTTP Digest__
This is a more secure form of the Basic Authentication and uses the MD5 hash for the password before encoding username and password with Base64. The server also creates a random value called nonce which will have to be sent with every request in addition to the encoded and encrypted username and password. The nonce will then be hashed with the password on the server and compared with the database.

It is more secure than HTTP Basic as it hashes the password instead of sending it in plain text format. This method does not provide a mechanism for logout, so the session lasts until the browser is closed. It is also vulnerable to man-in-the-middle attacks.


### 3.2 Session-based Authentication
For Session-based authentication the user state is stored on the server without requiring a username and password for each request. After logging in, the server validates the credentials once and generates a session that is stored in the session store. The session ID will be sent back to the client and used for all further requests done by the client. Each time a client requests the server, the server must locate the session in memory in order to tie the session ID back to the associated user. As the session ID is stored in a cookie on the client side, this is also called cookie-based authentication.

Credentials are only used once so after the initial login the following ones are faster. However, cookies are sent with every request now, no matter if they require authentication or not. The session store, which is used for storing user session information, needs to be shared across multiple services to enable authentication. Because of this, it doesn't work well for RESTful services since REST is a stateless protocol. This method is also vulnerable to CSRF attacks.

### 3.3 Token-based Authentication
This method does not need a session and is therefore well suited for single page applications and RESTful APIs. The server receives and validates the user credentials and then generates a token which contains the user information. This token will then be sent with every request to the server. It will not get stored on the server but can be validated by the signature which makes this method stateless. In the client it can be maintained in local storage, session storage or even in cookies.

Json Web Token (JWT) is the most commonly used implementation. A JWT consist of a header, a payload and a signature which are base64 encoded and concatenated. The header includes the token type and the hashing algorithm used. The payload includes the claims, which are statements about the subject. The signature is used to verify that the message wasn't changed along the way and signed with the private key.

This method is suited for a microservices architecture, where multiple services require authentication. Its stateless approach enables it to be used with REST. Since they are only decoded but not encrypted, everybody can decode and read them, but only authenticated users can create valid signed tokens. As tokens cannot be deleted, only expire, a leaked token can be misused until it expires. Depending on how the token is saved on the client, it can lead to XSS or CSRF attacks.

### 3.4 OpenID
OpenID is a protocol used for social login. It uses existing information from social networking services such as Facebook, Twitter, or Google to login.

The login screen of a website shows options such as ‘Sign in with Google’ or ‘Sign in with Facebook’. Clicking one of those will lead to an OpenID URL of the appropriate third-party service. A request is sent to the third-party service together with a shared secret to authenticate further communication between those parties. The user will get an HTTP redirect response to the third-party website and is prompted to log in there. After being authenticated there, the user will be redirected back to the original website and authenticated there automatically. This redirect will include information about the user from the third-party and the shared secret.

It can be useful if you are looking for a highly secure login, as these companies have enough resources to focus on authentication. First logins are also faster as they do not require the user to set up a new username and password. The downside of this is that your website is now dependent on another app which is outside of your control. If they are down, your users cannot log in. Additionally, users that do not have an account at one of the proposed third-party services, they are excluded from your website. For this reason, you should not offer OpenID exclusively, but always offer an additional authentication method.