---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/v1.0/education/users/13015"
requestBody.SetOdataId(&odataId) 

graphClient.Education().ClassesById("educationClass-id").Members().Ref().Post(context.Background(), requestBody, nil)


```