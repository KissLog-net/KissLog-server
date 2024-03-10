# KissLog server

## About

KissLog is a logging, exceptions tracking and Application Performance Monitoring server. <br/>
It provides a powerful and easy to use user-interface, allowing for viewing and analyzing the data in real time.

KissLog server ingests data via REST interfaces, making it compatible with any programming language and platform.

[kisslog.net](https://kisslog.net), the public instance of KissLog server, currently processes about 200 logs per second and a total of 50 million logs per month.

.NET applications can use the [KissLog.Sdk](https://github.com/KissLog-net/KissLog.Sdk) library which automatically sends all the logs and metrics to KissLog server.

### Technology

- Built on .NET6
- Working on Windows, Linux and Docker
- Uses MongoDB 6.0 or Azure Cosmos DB (as it can be hosted on Microsoft Azure)

## Artifacts

KissLog server artifacts can be downloaded from here: <br/>
<https://github.com/KissLog-net/KissLog-server/releases>

Installation and configuration guide can be found here: <br/>
[https://kisslog.net/Docs/on-premises.index.html](https://kisslog.net/Docs/on-premises.index.html)

### Latest versions

[KissLog.Frontend-v6.0.0-beta3](https://github.com/KissLog-net/KissLog-server/releases/tag/KissLog.Frontend-v6.0.0-beta3)

[KissLog.Backend-v6.0.0-beta3](https://github.com/KissLog-net/KissLog-server/releases/tag/KissLog.Backend-v6.0.0-beta3)

```none
docker pull catalingavan/kisslog.frontend:6.0.0-beta3
docker pull catalingavan/kisslog.backend:6.0.0-beta3
```

## Print screens

![Applications dashboard](https://user-images.githubusercontent.com/39127098/221179142-87a73564-f87d-46c2-b869-4019513cc010.png)
![Request details](https://user-images.githubusercontent.com/39127098/221179349-94676166-2f09-43f1-94d3-d272b5331086.png)
