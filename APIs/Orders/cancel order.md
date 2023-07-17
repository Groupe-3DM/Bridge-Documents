# Cancel an order

`Method: POST`


`endpoint: api/v1/orders/cancel`
### data body
````json
{
  "order_id": "required|exists:orders,id"
}
````
### data example
````json
{
  "order_id": "2104"
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