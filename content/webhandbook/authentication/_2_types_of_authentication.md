---
title: 2. Types of authentication
description : "Types of authentication"
tags: ["authentication", "types of authentication"]
---

A username or ID which is unique for each user is always required to determine their identity. If a client claims a specific identity, proof is required. Depending on the kind of proof that is required, authentication can be divided into three types: something you know, something you have, and something you are.

The most commonly used type of authentication would be a password, which makes it something that you know. Other examples of this type would be pattern, such as the ones used to unlock your smartphone, or graphical passwords where the correct interactions with a picture authenticate you. The problem is that it is easy to forget these passwords and users tend to choose easy passwords so that they can remember them.

Another type of authentication is something that you have. This could be hardware or software tokens, certificates, email, SMS, or USB keys. They either generate one-time passwords or a token which you can use to proof that you are who you say you are. Some automatically generate a new value every 30 or 60 seconds while other only generate a value when authentication is requested. The downside is that these device on which the tokens/OTPs are generated ca get lost or stolen.

Biometrics are the final type of authentication and defines something that you are. They can be either physical or behavioural. Physical biometrics include facial scan, fingerprint scan, or voice recognition.

Behavioural biometrics can be a signature, the way a person walks, or certain gestures. This type of authentication is more likely to be found in physical security and less in authentication on the web.

### 2.1 Password-based authentication
Password-based authentication is the most widely used type of authentication. For this type a password string following some predefined rules (have both lower- and upper-case letter, have numbers, have special characters etc.) is used together with the username to authenticate someone. The password is hashed, and preferably salted, and then stored in a database together with the username. When the user tries to log in with their credentials, the typed in password is hashed and salted and compared with the saved value in the database for this username. If they match, the user is authenticated.

One person normally has many different accounts for which they have to remember their password and remembering is difficult. As a result, many people choose convenience over security. They choose simple passwords that are easy to remember. Many even reuse the same password over multiple sites. Those simple passwords are easy and fast to crack with various methods and are prone to phishing attacks. Reusing passwords makes one leak affect multiple accounts.

Password managers have been created to help user’s choose complex passwords with less fear of forgetting them. The only thing the user has to remember is the master password which gives them access to all the saved passwords. So far this has only been done for text passwords.

### 2.2 Two-factor or multiple factor authentication
There is always the possibility to combine multiple authentication types. This is the case for 2-factor or multiple factor authentication. Most of the time these types of authentication use a password in combination with a user’s smartphone, Captcha tests or in some cases even biometrics such as fingerprints. While 2-factor authentication combines two independent ways to identify the user, multi-factor authentication uses even more.

One-time passwords or security tokens are most commonly used in combination with passwords. For this either a smartphone with an appropriate app or a hardware token device is needed. There are two ways the OTP can be generated on these devices: time-based or event-based. Time-based means that every 30 or 60 seconds a new value is generated. The same value is generated simultaneously, but independently from each other on your device as well as on the server. The value you type in must match the one on the server in order to authenticate you. Event-based OTPs are only generated when authentication is requested. The value is then sent to a device of your choice or to your email. This value has to be used for authentication and match the one saved on the server.

### 2.3 Certificate-based authentication
In comparison to biometrics and OTPs which only work for users, certificate-based authentication can be used to authenticate any kind of endpoint such as users, machine, devices and even the growing Internet of Things. A document called a public-key certificate is used to securely identify a user or other endpoint. It contains their public key and the digital signature of a certification authority. The server can then verify the credibility of the digital signature and the certificate authority and use the public key to check whether the private key used to sign the certificate is correct. It is often added to password use, thus making it a two-factor authentication without the hassle of doing any additional step as the certificate is automatically used for the authentication.