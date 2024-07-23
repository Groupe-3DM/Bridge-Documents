# Retrieve a purchase order 

### URL

```text
api/v1/purchase-orders/:id
```

### Method

```text
GET
```


### Note

```text

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