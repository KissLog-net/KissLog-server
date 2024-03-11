# KissLog server on Docker

KissLog server can run as a Docker container, thanks to [Marcio](https://github.com/zimbres) valuable contribution.

In this folder you will find all the necessary files.

```none
# starts the KissLog server and all the necesarry prerequisites
C:\KissLog-net\KissLog-server\Docker> docker-compose up

# stops the KissLog server docker containers
C:\KissLog-net\KissLog-server\Docker> docker-compose down

# Authentication token,
# a JWT signed with the value from frontend.KissLog.json@$.Authorization.HS256Secret
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.e30.HP79qro7bvfH7BneUy5jB9Owc_5D2UavFDulRETAl9E

# KissLog.Frontend endpoint
http://localhost:44080/

# KissLog.Backend endpoint
http://localhost:44088/
```

```csharp
// start sending the logs to the local KissLog.Backend endpoint
app.UseKissLogMiddleware(options => {
    options.Listeners.Add(new RequestLogsApiListener(new Application("_OrganizationId_","_ApplicationId_"))
    {
        ApiUrl = "http://localhost:44088/"
    });
});
```

<img width="642" alt="Login" src="https://github.com/KissLog-net/KissLog-server/assets/39127098/30b3b8bd-d7d4-4e79-9e5d-771df2f41174">

<img width="746" alt="Dashboard" src="https://github.com/KissLog-net/KissLog-server/assets/39127098/a50d654e-5a0b-4094-b328-63dad69f2e53">

<img width="746" alt="Request" src="https://github.com/KissLog-net/KissLog-server/assets/39127098/21517eae-a70b-4ccc-8277-f1314a2850ac">

<img width="746" alt="Windows terminal" src="https://github.com/KissLog-net/KissLog-server/assets/39127098/50c1adbf-7a1b-4cec-a22a-ceefdf9a91b7">

