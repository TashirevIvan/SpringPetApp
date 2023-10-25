# SpringPetApp
Для отправки запросов в формате JSON использовал Postman
#cURL:
#getAll
```
curl --location 'http://localhost:8989/getAll'
```
#getPet
```
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
```
#editPet
```
curl --location --request DELETE 'http://localhost:8989/deletePet' \
--header 'Content-Type: application/json' \
--data '{
    "id": 2
}'
```
#createPet
```
curl --location 'http://localhost:8989/createPet' \
--header 'Content-Type: application/json' \
--data '{
    "name": "Sharik",
    "type": "dog",
    "age": 2
}'
```
#deletePet
```
curl --location --request GET 'http://localhost:8989/getPet' \
--header 'Content-Type: application/json' \
--data '{
    "id": 1
}'
```
