# Create purchase order

`endpoint: api/v1/purchase-orders`

`Method: POST`

### Parameters

| Name                                     | Type    | Mandatory |
|------------------------------------------|---------|-----------|
| client_id                                | integer | Y         |
| shipping_method_id                       | string  | Y         |
| warehouse_id                             | integer | Y         |
| supplier_id                              | integer |           |
| date_expected                            | integer | Y         |
| po_number                                | integer | Y         |
| purchase_order_condition_id              | integer |           |
| purchase_order_status_id                 | integer |           |
| purchase_order_items                     | array   | Y         |
| purchase_order_items.*                   | array   | Y         |
| purchase_order_items.*.quantity_expected | integer | Y         |
| purchase_order_items.*.uom_quantity_id   | integer | Y         |
| purchase_order_items.*.item_id           | integer | Y         |
| purchase_order_items.*.lot               | integer |           |
| purchase_order_items.*.expiry_date       | date    |           |
| purchase_order_items.*.cost              | integer |           |
| purchase_order_items.*.lot               | integer |           |
| purchase_order_items.*.currency_id       | date    | Y         |
| purchase_order_items.*.subclient_id      | integer |           |
| purchase_order_items.*.upc               | integer |           |

### Response

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "po_number": "1-po-1701357058",
    "date_expected": "2021-09-01",
    "client_id": "1",
    "warehouse_id": 12,
    "client_name": "Group 3-DM",
    "supplier_id": null,
    "shipping_method_id": "1",
    "purchase_order_status_id": 1,
    "purchase_order_condition_id": 1,
    "id": 35,
    "warehouse_name": "3DM - AVRO",
    "purchase_order_items": [
      {
        "id": 43,
        "purchase_order_id": 35,
        "subclient_id": null,
        "item_id": 6,
        "cost": "3.0000",
        "currency_id": 1,
        "quantity_expected": 100,
        "quantity_received": 0,
        "supplier_code": "4",
        "lot": "",
        "upc": "2",
        "uom_type_id": 1,
        "purchase_order_item_status_id": 1,
        "uom_quantity": 1,
        "sku": "zxc",
        "client_id": 1,
        "quantity_in_progress": 0,
        "subclient": null
      }
    ]
  }
}
```