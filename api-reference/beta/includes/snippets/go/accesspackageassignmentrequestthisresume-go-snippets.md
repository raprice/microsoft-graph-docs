---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewResumePostRequestBody()
source := "Contoso.SodCheckProcess"
requestBody.SetSource(&source) 
type := "microsoft.graph.accessPackageCustomExtensionStage.assignmentRequestCreated"
requestBody.SetType(&type) 
data := graphmodels.NewCustomExtensionData()
additionalData := map[string]interface{}{
	"stage" : "assignmentRequestCreated", 
	"customExtensionStageInstanceId" : "957d0c50-466b-4840-bb5b-c92cea7141ff", 
	"customExtensionStageInstanceDetail" : "This user is all verified", 
}
data.SetAdditionalData(additionalData)
requestBody.SetData(data)

graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequestsById("accessPackageAssignmentRequest-id").Resume().Post(context.Background(), requestBody, nil)


```