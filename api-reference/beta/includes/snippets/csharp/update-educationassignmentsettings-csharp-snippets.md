---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentSettings = new EducationAssignmentSettings
{
	SubmissionAnimationDisabled = true
};

await graphClient.Education.Classes["{id}"].AssignmentSettings
	.Request()
	.UpdateAsync(educationAssignmentSettings);

```