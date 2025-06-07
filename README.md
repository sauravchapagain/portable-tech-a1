I have tried my best to host a two-tier web application manually and automate the same via Docker Compose.


some roughs 

docker run --name db -d -e MYSQL_ROOT_PASSWORD=pw 383946548058.dkr.ecr.us-east-1.amazonaws.com/db:latest



docker inspect sad_varahamihira |grep IPAddress


s3://s3-bucket-for-final-project/bg.jpg


docker run --name db -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=pw 383946548058.dkr.ecr.us-east-1.amazonaws.com/db:latest

docker run -p 81:81  -e DBHOST=172.17.0.2 -e DBPORT=$DBPORT -e  DBUSER=$DBUSER -e DBPWD=$DBPWD -e IMAGEURL=$IMAGEURL my_app

docker run -d --name app  -p 81:81  -e DBHOST=172.17.0.2 -e DBPORT=3306  -e DBPWD=pw -e APP_COLOR=blue IMAGEURL='s3://s3-bucket-for-final-project/bg.jpg
