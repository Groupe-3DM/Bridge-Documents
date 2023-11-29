# delete an order


`endpoint: api/v1/orders/delete/:id`

`Method: DELETE`

* `only if order status in (1 received, 2 released, 12 backorder, 14 receiving), can be deleted `
* `during the processing order, contact CSR directly`
# Response:

```json
{
    "success": true,
    "message": "Operation has been successfully completed!",
    "data": 0
}
```