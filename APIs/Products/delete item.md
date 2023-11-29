# delete an order

`Method: DELETE`


`endpoint: api/v1/orders/delete/:id`
### data body
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