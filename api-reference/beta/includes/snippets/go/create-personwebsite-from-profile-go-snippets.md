---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewPersonWebsite()
categories := []string {
	"football",

}
requestBody.SetCategories(categories)
displayName := "Lyn Damer"
requestBody.SetDisplayName(&displayName) 
webUrl := "www.lyndamer.no"
requestBody.SetWebUrl(&webUrl) 

result, err := graphClient.Me().Profile().Websites().Post(context.Background(), requestBody, nil)


```