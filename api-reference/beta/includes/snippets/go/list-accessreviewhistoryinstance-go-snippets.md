---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitionsById("accessReviewHistoryDefinition-id").Instances().Get(context.Background(), nil)


```