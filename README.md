# ASP.NET Core IdentityServer4
 
## An authorization server that can retrieve a token from it using different flows.

In summary the project deals with the following concepts:
* Token, Endpoint, and Flows
* Integration IdentityServer4 in the ASP.NET Core application
* The way to setup in-memory configuration
* How to retrieve tokens with different flows

## Testing Authorization Server

As you can see, we are using /connect/token endpoint to retrieve the token from the server. For parameters, we provide client-id, client_secret, password as a grant_type because we want to exchange user credentials for the token, and username and password. Once we press the Send button, we are going to receive our token:
![](https://github.com/Hunor85/asp-net-core-identity-server-4/blob/master/resources/img1.png)

Sometimes we don’t want to use the ResourceOwnerPassword flow but the ClientCredentials flow:
![](https://github.com/Hunor85/asp-net-core-identity-server-4/blob/master/resources/img2.png)
We have removed the user credentials and modified the grant_type to support client_credentials flow. As you can see, we can get the token.
