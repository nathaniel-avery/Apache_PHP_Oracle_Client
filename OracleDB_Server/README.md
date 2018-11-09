Configure and run an Oracle 12.2.0.1 container image

Download store/oracle/database-enterprise:12.2.0.1 image from oracle.  This might require you to logon.

Run the container

docker run -dit --name <name> -p 1521:1521 -p 5500:5500 store/oracle/database-enterprise:12.2.0.1

Note that this will expose the database on the host on port 1521 and the OEM on port 5500.  Errors will occur if the host is already using these ports.  To avoid a conflict, the exposed ports can be changed.

The database takes a few minutes to be created and start.  Progress can be checked by running
docker ps -a for a "healthy" status.  Also, the logs can be examined via the command

docker logs <name>

example:

docker run -dit --name oracle-ee -p 1521:1521 -p 5500:5500 store/oracle/database-enterprise:12.2.0.1

docker logs oracle-ee
