# import purchase orders

`endpoint: api/v1/import/purchase-orders`

`Method: POST`

### Parameters

| Name               | Type    | Mandatory |
|--------------------|---------|-----------|
| client_id          | integer | Y         |
| shipping_method_id | integer | Y         |
| warehouse_id       | integer | Y         |
| supplier_id        | integer |           |
| date_expected      | date    | Y         |
| po_number          | string  | Y         |
| sku                | string  | Y         |
| quantity_expected  | integer | Y         |
| uom_quantity_id    | integer | Y         |
| lot                | string  |           |
| expiry_date        | date    |           |
| cost               | decimal |           |
| currency_id        | date    | Y         |
| subclient_id       | integer |           |
| upc                | string  |           |

# response

```json
```