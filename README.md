# KissLog server

## About

KissLog server is an application which centralizes logs, exceptions and other related metrics produced by software applications. <br/>
It provides a user-friendly web interface for viewing and analyzing the data in real time.

KissLog server ingests data via REST interfaces, making it compatible with any programming language and platform.

[kisslog.net](https://kisslog.net), the public instance of KissLog server, currently processes about 200 logs per second and a total of 50 million logs per month.

.NET applications can use the [KissLog.Sdk](https://github.com/KissLog-net/KissLog.Sdk) library which automatically sends all the logs to KissLog server.

### Technology

- Built on .NET 6.0 framework
- Working on Microsoft, Linux and Docker
- Uses MongoDB 6.0 when hosted on IIS or Azure Cosmos DB when hosted on Microsoft Azure

## Artifacts

KissLog server artifacts can be downloaded from here: <br/>
<https://github.com/KissLog-net/KissLog-server/releases>

Installation and configuration guide can be found here: <br/>
[https://kisslog.net/Docs/on-premises.index.html](https://kisslog.net/Docs/on-premises.index.html)

### Latest versions

[KissLog.Frontend-v5.2.0-subscription02](https://github.com/KissLog-net/KissLog-server/releases/tag/KissLog.Frontend-v5.0.0)

[KissLog.Backend-v5.2.0-subscription02](https://github.com/KissLog-net/KissLog-server/releases/tag/KissLog.Backend-v5.1.0)

```none
docker pull catalingavan/kisslog.frontend:5.0.0
docker pull catalingavan/kisslog.backend:5.1.0
```

## Print screens

![Applications dashboard](https://user-images.githubusercontent.com/39127098/221179142-87a73564-f87d-46c2-b869-4019513cc010.png)
![Request details](https://user-images.githubusercontent.com/39127098/221179349-94676166-2f09-43f1-94d3-d272b5331086.png)
