# NATS demos
This repo contains the code for the demos that I use during sessions that I present about NATS and NATS Streaming.
The code is **NOT production grade** and only for demo purposes and for experimenting with NATS and NATS Streaming.

The repo contains the following demo projects:
- NATS
  - Basic messaging demos (pub/sub, request/response, queue-groups, wildcards).
- NATS-Streaming
  - BasicMessaging: basic messaging demo focussed on replaying messages.
  - Store: simple event-based distributed book-store application using NATS and NATS-Streaming.

> The Store demo assumes there is a SQL Server running on your local machine on port 1434. If you want to use a different host or port, change the connection-string in the 3 DBContext classes in the *OrderProcesingService*, *OrdersQueryService* and *ShippingService*. Also change the host and port on the *reset.ps1* script.