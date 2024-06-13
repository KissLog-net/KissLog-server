# KissLog server

The application has been renamed to logBee-app, and is currently maintained on https://github.com/catalingavan/logBee-app.

## About

KissLog is a logging, exceptions tracking and Application Performance Monitoring server. <br/>
It provides a powerful and easy to use user-interface, allowing for viewing and analyzing the data in real time.

KissLog server ingests data via REST interfaces, making it compatible with any programming language and platform.

[kisslog.net](https://kisslog.net), the public instance of KissLog server, currently processes about 200 logs per second and a total of 50 million logs per month.

### Technology

- Built on .NET6
- Working on Windows, Linux and [Docker](Docker/README.md)
- Uses MongoDB 6.0 or Azure Cosmos DB (as it can be hosted on Microsoft Azure)

## Artifacts

KissLog server artifacts can be downloaded from here: <br/>
<https://github.com/KissLog-net/KissLog-server/releases>

Installation and configuration guide can be found here: <br/>
[https://kisslog.net/Docs/on-premises.index.html](https://kisslog.net/Docs/on-premises.index.html)

### Latest versions

[KissLog.Frontend-v6.0.1](https://github.com/KissLog-net/KissLog-server/releases/tag/KissLog.Frontend-v6.0.1)

[KissLog.Backend-v6.0.1](https://github.com/KissLog-net/KissLog-server/releases/tag/KissLog.Backend-v6.0.1)

```none
docker pull catalingavan/kisslog.frontend:6.0.1
docker pull catalingavan/kisslog.backend:6.0.1
```

## Saving logs

- .NET applications can use the [KissLog.Sdk](https://github.com/KissLog-net/KissLog.Sdk) library which automatically sends all the logs and metrics to KissLog server

- Submitting logs by directly consuming the REST interface

```
POST http://localhost:44088/request-logs
{
  "organizationId": "_OrganizationId_",
  "applicationId": "_ApplicationId_",
  "startedAt": "2024-03-11T14:36:31.108Z",
  "durationInMilliseconds": 41,
  "httpProperties": {
    "absoluteUri": "http://localhost/catalog/createProduct?locale=en",
    "method": "POST",
    "response": {
      "statusCode": 200
    }
  },
  "logs": [
    {
      "logLevel": "Information",
      "message": "Creating product..."
    }
  ]
}
```

## User interface

<table><tr><td>
    <img alt="User interface" src="https://github.com/KissLog-net/KissLog-server/assets/39127098/8944691a-3f6e-4946-9a73-85390a867b87" />
</td></tr></table>

