---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')"
requestBody.SetOdataId(&odataId) 

graphClient.Policies().MobileAppManagementPoliciesById("mobilityManagementPolicy-id").IncludedGroups().Ref().Post(context.Background(), requestBody, nil)


```