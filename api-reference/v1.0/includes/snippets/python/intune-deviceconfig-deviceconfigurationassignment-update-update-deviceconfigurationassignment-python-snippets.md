---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = DeviceConfigurationAssignment(
	odata_type = "#microsoft.graph.deviceConfigurationAssignment",
	target = ConfigurationManagerCollectionAssignmentTarget(
		odata_type = "microsoft.graph.configurationManagerCollectionAssignmentTarget",
		collection_id = "Collection Id value",
	),
)

result = await graph_client.device_management.device_configurations.by_device_configuration_id('deviceConfiguration-id').assignments.by_assignment_id('deviceConfigurationAssignment-id').patch(body = request_body)


```