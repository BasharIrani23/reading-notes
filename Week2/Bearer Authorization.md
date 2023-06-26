
#Intro to JWT
### 1-What is a JSON Web Token (JWT)?
JWT is a compact and self-contained way of transmitting information between parties as a JSON object.

### 2- When should we use JSON Web Tokens?

JWTs are commonly used in authentication and authorization scenarios, where a user logs in and subsequent requests include the token to prove their identity and access privileges.
Claims are expected in which structural component of a JWT?

### 3-Claims are expected in the payload component of a JWT.
Claims are expected in the payload component of a JWT. The payload contains statements about an entity and additional data

# Are JWTs Secure?
### 1-If I get a JWT and I can decode the payload, how can we call that secure?
Just being able to decode the payload of a JWT doesn’t automatically make it secure. Security depends on how well the secret key used to sign the token is protected

### 2-If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature
When sending a JWT, both the sender and receiver need to know the secret key. It’s added to the signature part of the JWT and helps ensure its integrity.

### 3-Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.
The content and secret key should be shared through a secure channel. The recruiter should be instructed to store the secret key in a secure location, preferably offline and it's important 
to emphasize the need to keep the secret key confidential and not share it with anyone else.

#JWTs Explained
### 1- Why use JWT?
JWTs provide a secure way for authentication, authorization, and secure information exchange, making them a preferred choice in web and application development.

### 2-JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.
Imagine you have a backpack that you need to carry with you everywhere you go. Now, let's say this backpack is compact and lightweight, making it easy to carry around without feeling burdened.
You can take it with you wherever you need to go, whether it's to work, school, or a friend's house.
or imagine you have a box that contains all the information you need for a specific task. This box is compact, meaning it doesn’t take up much space. It’s also self-contained, meaning it holds everything you need without relying on anything external.

### 3-What are the three components (the structure) of a JWT signature?
-Header
-Payload
-Signature



