# inventory of sku details

### URL

```text
api/v1/inventories/item/details
```

### Method

```text
GET
```

### Parameters

| Name      | Type   | Required | Default | Description                          |
|-----------|--------|----------|---------|--------------------------------------|
| client_id | id     | Y        |         |
| sku       | string | Y        |         | string or strings separated by comma |

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

### Success Response

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": [
    {
      "sku": "sku1236",
      "item_id": 1,
      "total": 1486,
      "available": 1078,
      "receiving": 26,
      "on_hold": 0,
      "damaged": 2,
      "reserved": 368,
      "allocated": 12
    },
    {
      "sku": "JIF-321",
      "item_id": 2,
      "total": 2155,
      "available": 1061,
      "receiving": 0,
      "on_hold": 0,
      "damaged": 920,
      "reserved": 174,
      "allocated": 0
    }
  ]
}
```