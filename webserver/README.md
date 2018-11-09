These files create a container running an Apache webserver with PHP and the Oracle client.  

Execution instructions:

docker build -t <name> .
  
docker run -d -p 80:80 --name <name> <container id>

ex. docker run -d -p 80:80 --name mytestv69 c0eb6b61dc4a

The website can be validated by opening a web browser and going to http://localhost if the container host is your local machine.  Similarly, the PHP can be validated by opening a broweser and enterign the following URL http://localhost/hello.php
