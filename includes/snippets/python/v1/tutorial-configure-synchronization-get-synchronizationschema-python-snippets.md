---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)


request_configuration = SchemaRequestBuilder.SchemaRequestBuilderGetRequestConfiguration(
headers = {
		'Authorization' : "Bearer {Token}",
}

)

result = await graph_client.service_principals.by_service_principal_id('servicePrincipal-id').synchronization.jobs.by_job_id('synchronizationJob-id').schema.get(request_configuration = request_configuration)


```