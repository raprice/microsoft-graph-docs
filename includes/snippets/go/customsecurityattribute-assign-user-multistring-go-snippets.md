---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewUser()
customSecurityAttributes := graphmodels.NewCustomSecurityAttributeValue()
additionalData := map[string]interface{}{
engineering := graphmodels.New()
odataType := "#Collection(String)"
engineering.SetOdataType(&odataType) 
	project := []string {
		"Baker",
		"Cascade",

	}
	engineering.SetProject(project)
	customSecurityAttributes.SetEngineering(engineering)
}
customSecurityAttributes.SetAdditionalData(additionalData)
requestBody.SetCustomSecurityAttributes(customSecurityAttributes)

result, err := graphClient.UsersById("user-id").Patch(context.Background(), requestBody, nil)


```