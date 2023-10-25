# SpringPetApp
Для отправки запросов в формате JSON использовал Postman
cURL:
```
curl --location 'http://localhost:8989/getAll'

curl --location --request PUT 'http://localhost:8989/editPet' \
--header 'Content-Type: application/json' \
--data '{
    "1":{
    "name": "Barsik",
    "type": "cat",
    "age": 11
    },
    "2":{
    "name": "Sergey",
    "type": "capibara",
    "age": 2
    },
    "10":{
    "name": "Tomas",
    "type": "cat",
    "age": 422
    }
}'

curl --location --request DELETE 'http://localhost:8989/deletePet' \
--header 'Content-Type: application/json' \
--data '{
    "id": 2
}'

curl --location 'http://localhost:8989/createPet' \
--header 'Content-Type: application/json' \
--data '{
    "name": "Sharik",
    "type": "dog",
    "age": 2
}'

curl --location --request GET 'http://localhost:8989/getPet' \
--header 'Content-Type: application/json' \
--data '{
    "id": 1
}'
```
