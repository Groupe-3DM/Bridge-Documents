# Retrieve order shipping estimated cost information

### URL

```text
api/v1/orders/shipment/cost-estimated
```

### Method

```text
GET
```

### Parameters


| Name         | Type   | Required | Default | Description |
|--------------|--------|----------|---------|-------------|
| order_number | string | Y        |         |             |
| client_id    | index  | Y        |         |             |

### Note

```text

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
{
  "client_id": 1234,
  "order_number": "567890"
}
```

### Success response

```json
{
    "success": true,
    "message": "Operation has been successfully completed!",
    "data": {
        "cost": "8.89"
    }
}
```