# Cancel an order

`Method: POST`


`endpoint: api/v1/orders/cancel`

````json
{
  "order_id": "required|exists:orders,id"
}
````
# Response:

```json
{
    "success": true,
    "message": "Operation has been successfully completed!",
    "data": 0
}
```