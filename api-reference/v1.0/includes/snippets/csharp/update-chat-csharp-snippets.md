---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Chat
{
	Topic = "Group chat title update",
};
var result = await graphClient.Chats["{chat-id}"].PatchAsync(requestBody);


```