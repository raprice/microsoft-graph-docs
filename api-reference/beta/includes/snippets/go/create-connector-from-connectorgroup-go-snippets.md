---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
requestBody.SetOdataId(&odataId) 

graphClient.OnPremisesPublishingProfilesById("onPremisesPublishingProfile-id").ConnectorGroupsById("connectorGroup-id").Members().Ref().Post(context.Background(), requestBody, nil)


```