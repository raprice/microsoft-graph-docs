---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestFilter := "source eq 'Tenant'"

requestParameters := &graphconfig.SecurityAttackSimulationPayloadsRequestBuilderGetQueryParameters{
	Filter: &requestFilter,
}
configuration := &graphconfig.SecurityAttackSimulationPayloadsRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Security().AttackSimulation().Payloads().Get(context.Background(), configuration)


```