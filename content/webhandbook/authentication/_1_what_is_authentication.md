---
title: 1. What is authentication and why do we need it?
description : "What is authentication and why do we need it?"
tags: ["definition", "authentication"]
---

Authentication is the process of determining whether someone is who they say they are by checking to see if their credentials match the credentials in a database of authorized users. It is an important aspect of the security of a system and prevents unauthorized users from accessing sensitive data. It is even featured in the OWASP Top Ten Web Application Security Risks as ‘Identification and Authentication Failures’ in the 2021 version.

It should not be confused with authorization. While both terms are often used for the same thing and are implemented together, they describe different functions. Authentication is the process of verifying a user’s identity and determine whether the user should have access to the system or not. Authorization deals with access control and determines whether the user is allowed to access a specific resource they are requesting. Both are an integral part of an application’s security. However, this chapter focuses on authentication.

Authentication can be defined as a 3-step challenge-and-response process. First, the client claims an identity. Then, the server responds with a challenge and demands proof of this identity. Finally, the client supplies proof.

The most common form of proving one’s identity are a username and a password. However, there exist other additional types of authentications such as 2-factor or multiple factor authentication, hardware tokens or certificate-based authentication. Part 2 of this chapter will give you a quick overview of these types.

The web application protocols HTTP and HTTPS are stateless which means that theoretically the user would need to reauthenticate for each request. To simplify this there are different ways to generate a token for the user which will be send together with each request to authenticate them. Different methods to generate such a token will be explained in part 3 of this chapter.