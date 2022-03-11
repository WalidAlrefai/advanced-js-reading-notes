# Class 09

## Authorization/Authentication

**1- What header(s) are used in authentication and authorization**

The Authorization header is usually, but not always, sent after the user agent first attempts to request a protected resource without credentials.

The server responds with a 401 Unauthorized message that includes at least one WWW-Authenticate header. This header indicates what authentication schemes can be used to access the resource (and any additional information needed by the client to use them).

**2- What is safe to put into a JWT**

Only the server should know the "secret" that is used to generate the JWT. If someone modifies the data contained in the JWT, the server will fail to decode it. So the server can trust any JWT that it can decode.

However, if a hacker got access to your computer, they could see the JWT that is stored in the browser and use it. This same threat exists w/cookies, so it's not really a flaw of the JWT.

*One way to mitigate this threat is the expiration date of the JWT*. For a banking app, your JWT might expire after a few minutes. For Facebook, it might expire after a few months. However, there's no bullet proof solution to this if someone gets access to your browser.


**3- How are JWTs validated**

The rule of thumb is - you should always validate an incoming JWT. You should do it, even if you're working on an internal network - where the Authorization Server, the Client and the Resource Server aren't connected through the Internet. You shouldn't rely on your environment settings to be part of your security scheme. If you move your services to a public domain, the threat model will change and you will have to remember to update your security measures - experience shows that this is very often overlooked. Moreover, implementing token validation from the start will guard your from situations where someone manages to break into your network, or you would have a malicious actor in your organization.


## Term

**RBAC** is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments. A study by NIST has demonstrated that RBAC addresses many needs of commercial and government organizations. RBAC can be used to facilitate administration of security in large organizations with hundreds of users and thousands of permissions. Although RBAC is different from MAC and DAC access control frameworks, it can enforce these policies without any complication.

**User Roles** are permission sets that control access to areas and features within the Professional Archive Platform.

**JWT Token**  is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key.

