# Welcome to local database enviroment set up project!

Hi! 
As a developer we always work with various databases, and we may not want to install each of the database in local, so here is a solution for the problem.  
With the docker-compose files added here, we can actually run **Postgres**, **MySql** and **MsSql** server latest version at once with **persistent storage.**

# Files

1. [docker-compose.yml](https://github.com/LearnGrowAndShare/local-db-enviroment/blob/main/docker-compose.yml "docker-compose.yml") - To run **Postgres**, **MySql** and **MsSql** database server at once.
2. [mssql-docker-compose.yml](https://github.com/LearnGrowAndShare/local-db-enviroment/blob/main/mssql-docker-compose.yml "mssql-docker-compose.yml") - To run Ms SQL 2019 version database server.
3. [mysql-docker-compose.yml](https://github.com/LearnGrowAndShare/local-db-enviroment/blob/main/mysql-docker-compose.yml "mysql-docker-compose.yml") - To run MySql latest version database server.
4. [postgres-docker-compose.yml](https://github.com/LearnGrowAndShare/local-db-enviroment/blob/main/postgres-docker-compose.yml "postgres-docker-compose.yml") - To run Postgres Server latest version database server.

# Prerequisites 
1. [Docker](docker.com) 
2. Laptop with any operating system 

# How to run
We need to just run a single command to bring up all the database server at once.

> docker-compose up -d

Command prompt output-
![Command prompt output](https://github.com/LearnGrowAndShare/local-db-enviroment/docs/cmd-output.png)

Docker desktop output-
![Docker desktop output](https://github.com/LearnGrowAndShare/local-db-enviroment/docs/docker-desktop.png)

To run single database server, just specify {database_server}-docker-compose.yml
for example for mysql databas, we just have to run

> docker-compose -f mysql-docker-compose.yml  up -d

And to destroy all the instance we just have to change "*up*" with "*down*"

> docker-compose down

Happy coding... :smile:
