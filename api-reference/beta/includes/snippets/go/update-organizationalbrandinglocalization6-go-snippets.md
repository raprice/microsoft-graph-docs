---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewOrganizationalBrandingLocalization()
backgroundColor := "#00000F"
requestBody.SetBackgroundColor(&backgroundColor) 
signInPageText := "Welcome to Contoso France"
requestBody.SetSignInPageText(&signInPageText) 

result, err := graphClient.OrganizationById("organization-id").Branding().LocalizationsById("organizationalBrandingLocalization-id").Patch(context.Background(), requestBody, nil)


```