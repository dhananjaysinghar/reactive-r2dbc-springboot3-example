# reactive-r2dbc-springboot3-example


## Docker Command
~~~
docker run -p 5432:5432  --name postgresdb -e POSTGRES_PASSWORD=test_password -e POSTGRES_USER=test_user -e POSTGRES_DB=test_database --restart=always -d postgres

docker run -p 5050:80 --name pgadmin4 -e "PGADMIN_DEFAULT_EMAIL=dhananjaya.singhar@gmail.com" -e "PGADMIN_DEFAULT_PASSWORD=test_password"  -d dpage/pgadmin4


/etc/hosts 
host.docker.internal localhost
~~~

## POST API
~~~
curl --location 'http://localhost:8080/api/book' \
--header 'Content-Type: application/json' \
--data '{
    "source": "Bangelore",
    "destination": "Bhubaneswar",
    "date": "01/03/2023",
    "passengerName": "Dhananjay",
    "passengerAge": "33",
    "passengerGender": "M"
}'
~~~


## GET API 
~~~
curl --location --request GET 'http://localhost:8080/api/book/M573218281181816457' \
--header 'Content-Type: application/json'
~~~
