---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = CloudPcOnPremisesConnection(
	display_name = "test-canary-02",
	type = CloudPcOnPremisesConnectionType.HybridAzureADJoin,
	subscription_id = "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
	ad_domain_name = "contoso001.com",
	ad_domain_username = "dcadmin",
	organizational_unit = "OU=Domain Controllers, DC=contoso001, DC=com",
	resource_group_id = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG",
	virtual_network_id = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET",
	subnet_id = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet",
)

result = await graph_client.device_management.virtual_endpoint.on_premise_connections.post(body = request_body)


```