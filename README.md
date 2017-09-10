# Restaurant List API

### Get a list of all restaurants:
```
curl -s http://localhost:3000/api/v1/restaurants | jq
```
API gives response in the following format:
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
curl -s http://localhost:3000/api/v1/restaurants/2 | jq
```
API gives response in the following format:
```
{
  "id": 2,
  "name": "Wang Li",
  "address": "Laranjeiras",
  "comments": []
}
```
