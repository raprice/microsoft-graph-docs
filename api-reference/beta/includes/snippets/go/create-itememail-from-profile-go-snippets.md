---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewItemEmail()
address := "Innocenty.Popov@adventureworks.com"
requestBody.SetAddress(&address) 

result, err := graphClient.Me().Profile().Emails().Post(context.Background(), requestBody, nil)


```