# Status Codes


- In your own words, describe what each group of status code represents:
- - 100’s = information codes
- - 200’s = Success Codes
 - - 300’s = Redirection Codes
 - - 400’s = Client Error Codes
 - - 500’s = Server Error Codes


What is a status code 202?
- accepted response status code indicates that the request has been accepted for processing

What is a status code 308?
-  Permanent Redirect message

What code would you use if an update didn’t return data to a client?

- 204?

What code would you use if a resource used to exist but no longer does?

- 204

What is the ‘Forbidden’ status code?


- 403

# REST API With Mongo


Why do we need to pull our MongoDB database string out of our server and put it into our .env?

- It's the connection string

What is middleware?

- functions that execute during the lifecycle of a request to the Express server

What does app.use(express.json()) do?

- a builtin method in express to recognize the incoming Request Object as a JSON object.

What does the /:id mean in a route?

- Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.

What is the difference beween PUT and PATCH?

- PATCH supplies a set of instructions to modify the resource. PUT uses the request URI to spply a modified version of the requested resource which replaces the original version.

How do you make a defalut value in a schema?

-  date: { type: Date, default: '12/10/1990' }

What does a 500 error status code mean?

- Inernal Server Error

What is the difference between a status 200 and a status 201?

- 200 Means ok and gives data, 201 Means something on the server was created.
