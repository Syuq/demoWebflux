# api

## Create

```
curl --header "Content-Type: application/json" \
  --request POST \
  --data '{"title": "projectreactor","description": "xyz"}' \
  http://localhost:8080/api/tutorials
```

## Retrieve all

```
curl --header "Content-Type: application/json" \
  --request GET \
  http://localhost:8080/api/tutorials
```

## Update

```
curl --header "Content-Type: application/json" \
  --request PUT \
  --data '{"title": "projectreactor","description": "xyz","published": true}' \
  http://localhost:8080/api/tutorials/{id}
```

## Retrieve by Id

```
curl --header "Content-Type: application/json" \
  --request GET \
  http://localhost:8080/api/tutorials/{id}
```

## Find all published

```
curl --header "Content-Type: application/json" \
  --request GET \
  http://localhost:8080/api/tutorials/published
```

## Find all Tutorials which title contains a certain string:

```
curl --header "Content-Type: application/json" \
  --request GET \
  "http://localhost:8080/api/tutorials?title={String}"
```

## Delete

```
curl --header "Content-Type: application/json" \
  --request DELETE \
  http://localhost:8080/api/tutorials{id}
```

## Delete all

```
curl --header "Content-Type: application/json" \
  --request DELETE \
  http://localhost:8080/api/tutorials
```
