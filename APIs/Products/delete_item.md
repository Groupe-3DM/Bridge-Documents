# delete an order

### URL

```text
api/v1/items/:id
```

### Method

```text
DELETE
```

### Parameters

| Name                                | Type    | Required               | Default | Description |
|-------------------------------------|---------|------------------------|---------|-------------|
### Note

```text
* `any internal activities(inventory, receiving, return, order...) related can not be deleted`
```

### Auth required

```text
Yes
```

### Headers

```text
Content-Type: application/json
Accept: application/json
Authorization: Bearer ******************
```

### Request example

```json

```

### Success response

```json
{
    "success": true,
    "message": "Operation has been successfully completed!",
    "data": 0
}
```