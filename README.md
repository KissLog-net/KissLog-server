# KissLog server

## About

KissLog server is an application which centralizes logs, exceptions and other related metrics produced by software applications. <br/>
It provides a user-friendly web interface for viewing and analyzing the data in real time.

KissLog server ingests data via REST interfaces, making it compatible with any programming language and platform.

[kisslog.net](https://kisslog.net), the public instance of KissLog server, currently processes about 200 logs per second and a total of 50 million logs per month.

.NET applications can use the [KissLog.Sdk](https://github.com/KissLog-net/KissLog.Sdk) library which automatically sends all the logs to KissLog server.

## Artifacts

KissLog server artifacts can be downloaded from here: <br/>
<https://github.com/KissLog-net/KissLog-server/releases>

Installation and configuration guide can be found here: <br/>
[https://kisslog.net/Docs/on-premises.index.html](https://kisslog.net/Docs/on-premises.index.html)

### Latest versions

[KissLog.Frontend-v4.0.0-rc3](https://github.com/KissLog-net/KissLog-server/releases/tag/KissLog.Frontend-v4.0.0-rc3)

[KissLog.Backend-v4.0.0-rc3](https://github.com/KissLog-net/KissLog-server/releases/tag/KissLog.Backend-v4.0.0-rc3)

```none
docker pull catalingavan/kisslog.frontend:4.0.0-rc3
docker pull catalingavan/kisslog.backend:4.0.0-rc3
```
