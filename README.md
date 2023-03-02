# reactive-r2dbc-springboot3-example


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
