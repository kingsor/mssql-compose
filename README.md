# mssql-compose
Docker compose file for working with sql server 2019

I was using a sql server 2019 image in docker running this command:

```bash
docker run --name sqlserver-2019 -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=Ti6collegato!' -p 1433:1433 -d mcr.microsoft.com/mssql/server:2019-latest
```

and connecting with sql server with SqlServer Management Studio.

But I didn't used a volume and every time I restart my machine I have to restart the docker image.

So after a google search, I found this post

[Exploring SQL Server 2019 with Docker](https://espressocoder.com/2020/07/07/exploring-sql-server-2019-with-docker/)

where I got the docker-compose.yml file I was looking for.

