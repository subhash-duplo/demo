# demo
This is sample demo application to fetch and save the book into mysql DB

# My SQL
    Pull and run the docker container
        docker pull mysql:latest
        docker run -p 3307:3306 --name mysql -e MYSQL_ROOT_PASSWORD=root -d mysql:latest

    Connect to mysql server 
        mysql --host=<IP> --port=3307 -u root -proot
        e.g.  mysql --host=127.0.0.1 --port=3307 -u root -proot

    Create Database
        create database sample_db;

    Table and initial Data
        table will be created automatically on start-up of java application, just need to insert the few records later 

        insert into book values(1,'The India Story','Bimal Jalal');
        insert into book values(2,'Queen of Fire','Devika Rangachari');

# API 
    Get books
        GET /api/books
    Save book
        POST /api/books



