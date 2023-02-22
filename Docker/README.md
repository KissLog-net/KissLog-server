# KissLog server on Docker

KissLog server can be run as a Docker application, thanks to [Marcio](https://github.com/zimbres) valuable contribution.

In this folder you will find all the necessary files.

To spawn the KissLog server and all the necessary prerequisites, use `docker-compose up` command.

```none
C:\KissLog-net\KissLog-server\Docker> docker-compose up
```

After all the services have been created, you can access the applications on the following urls:

- KissLog.Frontend: <http://localhost:44080/>
- KissLog.Backend: <http://localhost:44088/>

To authenticate, use the following token:

```none
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.e30.FI5EFsgHo6MvkU7UXyu0wK6ZfpKA3y2vlVfmwFNEyMc@your.name.here
```

To destroy the services, use `docker-compose down` command.

```none
C:\KissLog-net\KissLog-server\Docker> docker-compose down
```

![docker-compose up](https://user-images.githubusercontent.com/39127098/220664267-b6d1235b-ee25-4e6e-bd6d-f93b562ada58.png)

![KissLog.Frontend login](https://user-images.githubusercontent.com/39127098/220663798-87427990-8c8c-4c79-8457-9f94bcaea25b.png)

![KissLog.Frontend applications](https://user-images.githubusercontent.com/39127098/220663936-745dfa57-7b11-4bbf-a937-b5a169655002.png)