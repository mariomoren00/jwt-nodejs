# Jwt with nodejs

Using nodejs with express and jwt authentication

This repo uses JSON Web Tokens and the jsonwebtoken package to implement token based authentication on a simple Node.js API.

This is a starting point to demonstrate the method of authentication by verifying a token using Express route middleware.

Getting a Token

Send a POST request to http://localhost:8080/api/authenticate with test user parameters as x-www-form-urlencoded.

  {
    name: 'Mario Moreno',
    password: 'password'
  }
  
Verifying a Token and Listing Users

Send a GET request to http://localhost:8080/api/users with a header parameter of x-access-token and the token.

You can also send the token as a URL parameter: http://localhost:8080/api/users?token=YOUR_TOKEN_HERE

Or you can send the token as a POST parameter of token.
