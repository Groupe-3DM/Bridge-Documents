# delete an order

### URL

```text
api/v1/orders/delete/:id
```

### Method

```text
DELETE
```

### Parameters

| Name                           | Type    | Required | Default | Description |
|--------------------------------|---------|----------|---------|-------------|


### Note
```text
only if order status in (1 received, 2 released, 12 backorder, 14 receiving), can be deleted

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