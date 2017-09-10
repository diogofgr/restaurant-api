# Restaurant List API

### Get a list of all restaurants:

```
curl -s https://restaurant-list.herokuapp.com/api/v1/restaurants | jq
```
or if you are developing locally:
```
curl -s http://localhost:3000/api/v1/restaurants | jq
```
The API gives response in the following format:
```
[
  {
    "id": 1,
    "name": "McDonalds",
    "address": "Carcavelos"
  },
  {
    "id": 2,
    "name": "Wang Li",
    "address": "Laranjeiras"
  }
]

```

### Get details of the restaurant with ` id: 2 `:
```
curl -s https://restaurant-list.herokuapp.com/api/v1/restaurants/2 | jq
```
or if you are developing locally:
```
curl -s http://localhost:3000/api/v1/restaurants/2 | jq
```
The API gives response in the following format:
```
{
  "id": 2,
  "name": "Wang Li",
  "address": "Laranjeiras",
  "comments": []
}
```
