---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthenticationMethodConfiguration
{
	OdataType = "#microsoft.graph.softwareOathAuthenticationMethodConfiguration",
	State = AuthenticationMethodState.Disabled,
};
var result = await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"].PatchAsync(requestBody);


```