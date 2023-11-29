# Cancel an order

`endpoint: api/v1/orders/cancel`

`Method: POST`

### Parameters:

| Name     | Type      | Mandatory |
|----------|-----------|-----------|
| order_id | integer   | Y         |

* `only if order status in (1 received, 2 released, 12 backorder, 14 receiving), can be cancelled `
* `during the processing order, contact CSR directly`

### Response

```json
{
    "success": true,
    "message": "Operation has been successfully completed!",
    "data": 0
}
```