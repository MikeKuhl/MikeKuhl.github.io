# What is OAuth?
- OAuth is an authentication protocol that allows you to approve one application interacting with another on your behalf without giving away your password.
Give an example of what using OAuth would look like.
- Using your Github account to log into code katas or Freecodecamp.
How does OAuth work? What are the steps that it takes to authenticate the user?
What is OpenID?
- Instead of sharing passwords, it authenticates the permission to perform actions with an authroized token. So the user requests, gets permission, once the user is given an access token they are given access. OpenID is an authentication layer for OATUH.


# Authentication


What is the difference between authorization and authentication?
- Authentication, telling the system who you are and providing credentials. Authorization allows you to do things because of who you are.

What is Authorization Code Flow?
- ![authorization-code-flow](https://images.ctfassets.net/cdy7uua7fh8z/2nbNztohyR7uMcZmnUt0VU/2c017d2a2a2cdd80f097554d33ff72dd/auth-sequence-auth-code.png)
What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
- ```
The user clicks Login within the application.

Auth0's SDK creates a cryptographically-random code_verifier and from this generates a code_challenge.

Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) along with the code_challenge.

Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the application.

Your Auth0 Authorization Server stores the code_challenge and redirects the user back to the application with an authorization code, which is good for one use.

Auth0's SDK sends this code and the code_verifier (created in step 2) to the Auth0 Authorization Server (/oauth/token endpoint).

Your Auth0 Authorization Server verifies the code_challenge and code_verifier.

Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

Your application can use the Access Token to call an API to access information about the user.

The API responds with requested data.
```
What is Implicit Flow with Form Post?
- Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls.
What is Client Credentials Flow?
- in the client credentials flow, permissions are granted directly to the application itself by an administrator
What is Device Authorization Flow?
-  that enables devices with no browser or limited input capability to obtain an access token.
What is Resource Owner Password Flow?
- allows you to keep separate user directories (which map to separate connections) and specify which one to use during the flow.

