1.  Write the following steps in the correct order:
-   Register your application to get a client_id and client_secret
-   Ask the client if they want to sign in via a third party
-   Redirect to a third party authentication endpoint
-  Receive access token
-  Receive authorization code
- Make a request to the access token endpoint
-  Redirect to a third party authentication endpoint
3.  What can you do with an authorization code?
	* The client can recieve an access token*
4.  What can you do with an access token?
* The user can access their own secured data
6.  What’s a benefit of using OAuth instead of your own basic authentication?
	* Allows for access to multiple services with one Access token.


### Define

Client ID - Unique User or device ID for the client.

Client Secret - used to authenticate to the auth server.

Authentication Endpoint - endpoint that only authorized clients can connect or access.

Access Token Endpoint - The token endpoint is **where apps make a request to get an access token for a user**.

API Endpoint -  the code that allows two software programs to communicate with each other -- connects with the software program

Authorization Code - password that user needs to access

Access Token - Object that encapsulate the secured information of a user.