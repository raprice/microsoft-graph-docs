---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewSnoozeReminderPostRequestBody()
newReminderTime := graphmodels.NewDateTimeTimeZone()
dateTime := "dateTime-value"
newReminderTime.SetDateTime(&dateTime) 
timeZone := "timeZone-value"
newReminderTime.SetTimeZone(&timeZone) 
requestBody.SetNewReminderTime(newReminderTime)

graphClient.Me().EventsById("event-id").SnoozeReminder().Post(context.Background(), requestBody, nil)


```