# 5 steps to RBAC 
### 1-What is Role Based Access Control (RBAC) and why do we care?
Role-Based Access Control (RBAC) is a security model used to manage and control access to resources within an organization's systems. It is based on the concept of assigning permissions and privileges to specific roles rather than individual users.
Users are then assigned to roles based on their job responsibilities or functions within the organization.
### 2-Describe a Role/Permission heirarchy that you might implement using RBAC.
- Superadmin :This role has full access and control over all resources and functionalities within the system.
- Admin Role:The admin role has permissions to manage user accounts, roles, and system configurations
- Manager Role:Managers have permissions to access and manage specific departments or teams within the organization
- User Role: Users have basic permissions to perform their regular job functions.
- Guest Role :Guests have limited access to the system and are typically restricted to publicly available information or certain non-sensitive resources.
### 3-What approach might you take to implement RBAC?
The implementation of RBAC can vary based on the specific requirements of the organization and the technology stack employed
***

# wiki - RBAC
### 1- If Authentication is “you are who you say you are,” what is Authorization?
Authorization is the process of granting or denying access rights to a user based on their authenticated identity.
### 2- Name three primary rules defined for RBAC.
- Role assignment
- Role permission
- Role authorization
### 3-Describe RBAC to a non-technical friend.
RBAC, which stands for Role-Based Access Control, is a way to manage and control who can access certain things in a system or organization.
Imagine you have a big office building with different rooms and areas, and you want to control who can enter each room and what they can do inside.
In RBAC, we assign specific roles to different people based on their job or responsibilities. 
***
# RBAC tutorial
### 1- What Are access rights Associated with? The User? or The Role? Explain.
Access rights in RBAC are associated with roles, not individual users. This means that users are assigned roles, and the permissions associated with those roles determine their access rights. In other words, the permissions are linked to roles, and users inherit the access rights based on the roles they are assigned.
### 2- Access Rights, or Authorization, is activated after a user successfully does what?
Access Rights, or Authorization, is activated after a user successfully authenticates or verifies their identity. Once the user has proven that they are who they claim to be through the authentication process, the system can then activate the authorization process to determine the user's access rights. It is the combination of successful authentication followed by authorization that allows the user to access specific resources, perform certain actions, or utilize functionalities within a system or organization.
### 3-Explain how RBAC might benefit a business
- Enhanced Security :RBAC helps improve security by ensuring that users have appropriate access rights based on their roles and responsibilities
- Scalability and Flexibility: RBAC provides scalability as organizations grow and evolve. New roles can be defined and assigned
- Access Control Simplification: RBAC simplifies access management by assigning permissions to roles rather than individual users.













