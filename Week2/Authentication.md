# Securing Passwords
### 1-Explain to a non-technical friend how you would safely hash and store a password.

When it comes to safely hashing and storing a password, here's how I would explain the process to a non-technical friend
- Hashing: We convert the password into a unique and irreversible string.
- Salt: We add a random string to the password before hashing to make it harder to crack.
- Secure Algorithm: We use a strong and slow algorithm to hash the password securely.
- Storage: We store the hashed password in a database.
By using these techniques, we make it difficult for attackers to retrieve the original password even if they gain access to the stored data.

### 2-What is Bcrypt?

bcrypt is a widely used and secure cryptographic hashing algorithm designed for password hashing. It is specifically designed to be slow and computationally intensive, making it difficult for attackers to quickly crack hashed passwords through brute-force or dictionary attacks.

### 3- Why might you use something like Bcrypt?
Bcrypt is used for secure password hashing. It makes it difficult for attackers to crack passwords and enhances overall system security. It is a recommended industry practice for storing passwords securely.

# Basic Auth
### 1- What is Basic Authentication?
Basic Authentication is a simple and widely supported method used for authenticating and authorizing users in web applications and APIs. It involves sending the user's credentials (username and password) in the HTTP request headers.

### 2-What properties are necessary in the header of a Basic Auth request?

In the header of a Basic Authentication request, the "Authorization" property is necessary. It consists of the following components:

- Authorization: The "Authorization" property is used to specify the type of authentication being used, which in this case is "Basic". It is followed by a space.

- Credentials: The "Credentials" property contains the encoded username and password, separated by a colon (":"). This value is then Base64 encoded.
- 
### 3-How are username:password in Basic Auth encoded?
In Basic Authentication, the username and password are encoded using Base64 encoding. 

# OWASP auth cheatsheet
### 1- Define the authentication process to a non-technical recruiter.
Authentication is the process of verifying the identity of a user or entity to ensure they are who they claim to be. 
Authentication is essential for ensuring that only authorized individuals can access sensitive data, systems, or resources.

### 2-How should your error messaging respond (both HTTP and HTML)? Why?
Error messaging, both in HTTP responses and HTML pages, should be informative and user-friendly. why it's important ? it giving a clear and informative error messaging is important because it helps users understand and resolve issues, enhances user experience, and reduces frustration.

### 3-Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.

Bookmark this link for reference on secure authentication practices (OWASP). It helps create more secure applications by following established security guidelines.





