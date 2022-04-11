# DataversePostmanCollection
A template for using the Dataverse Web API in Postman, where connection is made using an Application User

Postman can be really useful in testing out API calls during development, to construct complex queries and testing out credentials. Problem is, I keep forgetting exactly what to do in order to create the postman environment. The instructions on Microsoft Docs use user credentials, but for creating applications it's best practice to create an application user: https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#create-an-application-user

I've created a basic Postman Environment for connecting with an application user. All you need to fill is the url, clientid, clientsecret and directoryid (the Tenant Id in Azure Active Directory). In the Postman Collection I've added a "Get Access Token" Request, that when succesful saves the Access Token in the Environment. The Query Example Request uses the saved access token.
