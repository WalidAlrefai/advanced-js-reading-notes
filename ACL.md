# Class08
## Access Control (ACL):
**role-based access control (RBAC) or role-based security** is an approach to restricting system access to authorized users. It is an approach to implement mandatory access control (MAC) or discretionary access control (DAC).

**Role-based access control (RBAC)** is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments. A study by NIST has demonstrated that RBAC addresses many needs of commercial and government organizations. RBAC can be used to facilitate administration of security in large organizations with hundreds of users and thousands of permissions. Although RBAC is different from MAC and DAC access control frameworks, it can enforce these policies without any complication.

### What are Examples of RBAC?
Through RBAC, you can control what end-users can do at board and granular levels. You can designate whether the user is an administrator or standard user, and align roles and permissions based on the user's position in the organization.

The core principle is to allocate only enough access for an employee to do their job.

If the employee's job changes, you may need to add and/or remove them for their current role group.

By adding a user to a role group, the user has access to all the permissions of that group. If they are removed, access becomes restricted. Users can also be assigned temporary access to certain data or programs to complete a task and be removed after.

Common examples of RBAC include:

Software engineering role: Has access to GCP, AWS, and GitHub Marketing role: Has access to HubSpot, Google Analytics, Facebook Ads, and Google Ads Finance role: Has access to Xero and ADP Human resources role: Has access to Lever and BambooHR



### What are the advantages of RBAC?

1- The assignment of access privileges becomes systematic and repeatable with the proper deployment of RBAC. Furthermore, auditing user permissions and correcting any errors discovered is significantly easier.

2- RBAC may appear frightening, but it is actually rather simple to deploy and will make access rights management more easier and more secure.

### The Implementation of RBAC

1- Inventory your systems
If you don't already have a list of resources for which you need to manage access, make one now. An email system, a customer database, a contact management system, and significant directories on a file server are all examples.

2- Analyze your workforce and create roles
You should organize your employees into roles with similar access requirements. Don't succumb to the temptation of having too many jobs specified. Maintain as much simplicity and stratification as feasible. For example, a basic user position would have access to email and the intranet site, which every employee would require. A customer care representative with read/write access to the customer database and a customer database administrator with full control of the customer database are two alternative roles that could be considered.

3- Assign people to roles
Determine which role(s) each employee belongs in, and adjust their access accordingly, now that you have a list of roles and their access rights.

4- Never make one-off changes
If an employee has special needs, resist the urge to make a one-time adjustment. Your RBAC system will swiftly fall apart if you start doing this. Change the roles as needed, or create new ones as needed.

5-Audit
Review your positions, the personnel assigned to them, and the access granted to each on a regular basis. If you find that a role has unneeded access to a system, for example, alter the role and adjust the access level for all employees in that job.


## Term
- encryption: Encryption is a method of securing digital data that involves the use of one or more mathematical procedures, as well as a password or "key" to decrypt the data. The encryption procedure converts data using an algorithm that renders the original data unreadable.

- Access: Access tokens are used by programs to make API queries on a user's behalf. The access token denotes a certain application's permission to access specified elements of a user's data.

- bearer: The most common type of access token used with OAuth 2.0 is a Bearer. A Bearer Token is an obfuscated string that has no meaning for the clients who use it. Some servers will utilize a short string of hexadecimal characters as tokens, while others will employ structured tokens like JSON Web Tokens.

- secret: is a password that only the application and the authorization server have access to.

- JSON Web Token: JSON Web Token (JWT) is a URL-safe way of representing claims to be transferred between two parties in a compact format.


## Review, Research, and Discussion
- **When is Basic Authorization used vs. Bearer Authorization?**

The Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret. The Bearer authentication scheme is dedicated to the authentication using a token.

Instead of having your user send their actual credentials to your server on every single request (like they would with Basic Auth, where a user sends their username/password to the server for each request), with OAuth you first exchange your user credentials for a 'token', and then authenticate users based on this token.

- **What does the JSON Web Token package do?**

Each JWT contains encoded JSON objects, including a set of claims. JWTs are signed using a cryptographic algorithm to ensure that the claims cannot be altered after the token is issued.

- **What considerations should we make when creating and storing a SECRET?**

a. Differentiate Between Secrets and Identifiers.
b. Establish a Circle of Trust.
c. Encrypt Data Using a KMS.
d. Detect Unauthorized Access.

