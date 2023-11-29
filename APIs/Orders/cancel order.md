# Cancel an order

`endpoint: api/v1/orders/cancel`

`Method: POST`

### Parameters:

| Name     | Type      | Mandatory |
|----------|-----------|-----------|
| order_id | integer   | Y         |

### Response

```json
{
    "success": true,
    "message": "Operation has been successfully completed!",
    "data": 0
}
```