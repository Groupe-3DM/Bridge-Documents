# Preate purchase order

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

# response

```json
```