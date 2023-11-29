# delete an order

`Method: DELETE`


`endpoint: api/v1/items/:id`

* `any internal activities(inventory, receiving, return, order...) related can not be deleted`

# Response:

```json
{
    "success": true,
    "message": "Operation has been successfully completed!",
    "data": 0
}
```