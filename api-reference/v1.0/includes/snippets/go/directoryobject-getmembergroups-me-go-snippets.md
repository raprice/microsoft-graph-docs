---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewGetMemberGroupsPostRequestBody()
securityEnabledOnly := true
requestBody.SetSecurityEnabledOnly(&securityEnabledOnly) 

result, err := graphClient.Me().GetMemberGroups().Post(context.Background(), requestBody, nil)


```