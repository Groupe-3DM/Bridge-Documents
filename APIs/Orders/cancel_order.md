# Cancel an order

### URL

```text
api/v1/orders/cancel
```

### Method

```text
POST
```

### Parameters

| Name     | Type    | Required | Default | Description                                                                                      |
|----------|---------|----------|---------|--------------------------------------------------------------------------------------------------|
| order_id | integer | Y        |         | order with order_status_id: 1 received, 2 released, 12 backorder, 14 receiving, can be cancelled |

### Note
```text
during the processing order, contact CSR directly
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