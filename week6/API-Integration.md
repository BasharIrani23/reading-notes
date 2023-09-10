# Review API Server Build
### 1-Explain the different between a query string parameter and a path parameter.

A query string parameter and a path parameter are both methods of sending data in an HTTP request, but they have different structures and purposes:

Path Parameter: It is part of the actual URL path. Typically used to identify a specific resource or a set of resources. They are embedded in the URL. For example, in the URL http://amazingapi.com/api/v1/products/12345, 12345 is a path parameter that likely identifies a unique product.

Query String Parameter: It comes after the main URL path and is typically used to send non-unique values that the server can use to process the request. They start with a ? and are in the format key=value. Multiple query parameters are separated by &. For example, in the URL http://amazingapi.com/api/v1/products?category=electronics, category=electronics is a query string parameter that filters products by the electronics category.

### 2-What would our API URL with a path id parameter be given the following information:
Given the domain, version, model name, and id provided, the URL would be:

bashCopy code
http://our-site.com/api/v3/stuff/things
Description of the dynamic API with an "interface":


### 3-We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.
Alright, imagine you have a universal remote control that can operate any brand or type of device – TV, DVD player, air conditioner, and so on. Instead of having different remote controls for each device, you have this one remote that can connect to anything.

Our dynamic API is like that universal remote. No matter what kind of data (like TV, DVD, etc.) we want to manage, our API can handle it. The "interface" is like the buttons on the remote. Just as the play button always plays, regardless of the device brand, our API always knows how to perform actions like add, remove, or retrieve data, no matter what kind of data it is.

So, in simple words, we've made a super-smart system that can work with any data we give it, much like a universal remote can work with any device.
*** 
# Review Auth Server Build

### 1-Describe how you would use middleware to implement basic and bearer auth.

Middleware functions are functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. Middleware allows us to intercept or modify requests before they reach their intended route handlers.

Basic Authentication:

The client sends a request with an Authorization header containing the word Basic followed by a space and a base64-encoded username:password string.
The BasicAuth middleware decodes the base64 string to retrieve the original username and password.
Using the provided username, it queries the database to retrieve the corresponding user.
If the user is found, it checks the provided password against the stored hashed password in the database.
If the credentials are valid, the user is considered authenticated and the request can proceed. If not, an authentication error is sent back.
Bearer Authentication:

After the user logs in, the server provides a token (often JWT or similar).
In subsequent requests, the client includes this token in the Authorization header with the prefix Bearer.
The BearerAuth middleware extracts this token and verifies it (checks its signature, expiry date, etc.).
If the token is valid, the middleware extracts user information from it, and the user is considered authenticated.
If the token is invalid, an authentication error is returned.
In both cases, if authentication is successful, we can attach the user object or relevant user details to the request object (req.user) to be used in subsequent middleware or route handlers.

### 2-Describe the handshake necessary to implement OAuth.

OAuth is a process that allows a user to grant a third-party application limited access to their resources, without sharing their credentials. 

*Here's a basic overview of the OAuth handshake:*

- Initiation: The user initiates the process by clicking something like "Login with Google".

- Redirect: The application redirects the user to the OAuth provider's authorization page. This page asks the user if they are willing to grant the requesting app the permissions it's asking for.

- Authorization: If the user agrees, the OAuth provider sends a one-time code to the application's registered callback URL.

- Token Exchange: The application then exchanges this one-time code for an access token by making a server-to-server request, providing its client ID, client secret, and the one-time code.

- Access Granted: With this access token, the application can make requests to access the user's resources until the token expires or is revoked by the user.


### 3-Describe how Role Based Access Control works to a non-technical friend.

Imagine you're at a music concert. When you enter, you get a wristband. There are different types of wristbands:

- General Admission: Lets you access only the main areas.
- VIP: Lets you access the main areas and the VIP lounge.
- Artist: Lets you access the main areas, VIP lounge, and backstage.
- Crew: Allows you everywhere, including on stage and technical areas.
- Role-Based Access Control (RBAC) is like those wristbands, but for computer systems. Instead of physical areas, we have parts of a system or actions you can perform. And instead of wristbands, users are assigned roles like "Admin", "Editor", or "User". Each role has specific permissions:

- Admin might be able to read, edit, create, and delete data.
- Editor might be able to read, edit, and create, but not delete.
- User might only be able to read.
When a user tries to do something, the system checks their "wristband" (role) to see if they're allowed. If they have the right role, they're in; if not, they're denied access. This way, we ensure everyone can only do what they're supposed to.
