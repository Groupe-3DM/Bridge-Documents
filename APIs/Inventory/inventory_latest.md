# Latest modified Inventory


`Method: GET`

`endpoint: api/v1/inventory/item/latest-modified`

### parameters:
| Name        | Type      | mandatory  |
|-------------|-----------|------------|
| client_id   | integer   | Y          |


# response

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": [
    {
      "sku": "sku1236",
      "item_id": 1,
      "qty": 1026
    }
  ]
}
```