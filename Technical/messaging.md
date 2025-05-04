# Messaging

## Comparison of services

The following table compares the three services: Event Grid, Event Hubs, and Service Bus.

| Service | Purpose | Type | When to use |
| --- | --- | --- | --- |
| Event Grid | Reactive programming | Event distribution (discrete events) | React to status changes |
| Event Hubs | Big data pipeline | Event streaming (series) | Telemetry and distributed data streaming |
| Service Bus | High-value enterprise messaging | Message | Order processing and financial transactions |

### Use the services together

In some cases, you use the services side by side to fulfill distinct roles. For example, an e-commerce site can use Service Bus to process the order, Event Hubs to capture site telemetry, and Event Grid to respond to events like an item was shipped.
In other cases, you link them together to form an event and data pipeline. You use Event Grid to respond to events in the other services. For an example of using Event Grid with Event Hubs to migrate data to Azure Synapse Analytics, see Stream big data into Azure Synapse Analytics. The following image shows the workflow for streaming the data.
