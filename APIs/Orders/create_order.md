# Create an order

### URL

```text
api/v1/orders
```

### Method

```text
POST
```

### Parameters

| Name                           | Type    | Required                 | Default | Description                        |
|--------------------------------|---------|--------------------------|---------|------------------------------------|
| client_id                      | id      | Y                        |         |                                    |
| order_number                   | string  |                          |         |                                    |
| order_date                     | string  | Y                        |         |                                    |
| first_name                     | string  | Y                        |         |                                    |
| last_name                      | string  |                          |         |                                    |
| apt_num1                       | string  |                          |         |                                    |
| apt_num2                       | string  |                          |         |                                    |
| address1                       | string  | Y                        |         | max 35 characters                  |
| address2                       | string  |                          |         | max 35 characters                  |
| city                           | string  | Y                        |         |                                    |
| province_id                    | id/code | Y                        |         | [APIs](../Others/get_provinces.md) |
| country_id                     | id/iso2 | Y                        |         | [APIs](../Others/get_countries.md) |
| company                        | string  |                          |         |                                    |
| telephone                      | string  |                          |         |                                    |
| email                          | email   |                          |         |                                    |
| postal_code                    | string  | Y                        |         |                                    |
| reference1                     | string  |                          |         |                                    |
| reference2                     | string  |                          |         |                                    |
| note                           | string  |                          |         |                                    |
| custom_reference_no            | string  |                          |         |                                    |
| packing_slip_note              | string  |                          |         |                                    |
| order_items                    | array   | Y                        |         |                                    |
| order_items.*                  | array   | Y                        |         |                                    |
| order_items.*.quantity_ordered | integer | Y                        |         |                                    |
| order_items.*.uom_type_id      | id      | Y                        |         | [APIs](../Others/get_uom_types.md) |
| order_items.*.item_id          | id      |                          |         | [APIs](../Products/get_items.md)   |
| order_items.*.sku              | string  | Y if item_id not present |         |                                    |
| order_items.*.lot              | string  |                          |         |                                    |
| order_items.*.expiry_date      | date    |                          |         |                                    |
| order_items.*.unit_value       | integer |                          |         |                                    |

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
{
  "client_id": 1,
  "order_date": "2023-09-09 11:11:11",
  "email": "test@email.com",
  "first_name": "john",
  "last_name": "Don",
  "address1": "222 ave mntril",
  "address2": "",
  "province_id": "QC",
  "country_id": "CA",
  "city": "Montreal",
  "postal_code": "H9R 3S4",
  "order_items": [
    {
      "sku": "aipods2",
      "quantity_ordered": 1,
      "uom_type_id": 1
    }
  ]
}
```

### Success response

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "client_id": 1,
    "client_name": "GROUPE 3-DM",
    "order_number": 1709755068,
    "client_order_id": null,
    "order_date": "2023-09-09 11:11:11",
    "email": "test@email.com",
    "first_name": "john",
    "last_name": "Don",
    "address1": "222 ave mntril",
    "province_id": 612,
    "country_id": 38,
    "city": "Montreal",
    "telephone": null,
    "company": null,
    "postal_code": "H9R 3S4",
    "address2": null,
    "address3": null,
    "apt_num1": null,
    "apt_num2": null,
    "reference1": null,
    "reference2": null,
    "parent_id": null,
    "packing_slip_note": null,
    "handling_priority": 0,
    "processing_priority": false,
    "is_master": false,
    "ready": 0,
    "order_type_id": 1,
    "order_status_id": 1,
    "pick_up": false,
    "inside_delivery": false,
    "lift_gate_required": false,
    "hazmat": false,
    "order_handling": false,
    "appointment_required": false,
    "temperature_control": false,
    "dangerous_goods": false,
    "language_id": 1,
    "warehouse_id": "11",
    "department_id": 2,
    "rates_shop": 0,
    "carrier_id": 1,
    "transaction": null,
    "carrier_service": null,
    "service_id": null,
    "note": null,
    "custom_reference_no": null,
    "created_by": "Genming Zhao",
    "updated_by": "Genming Zhao",
    "deliver_by_date": null,
    "signature_required": false,
    "ambient_control": false,
    "air_ground_control": 0,
    "ship_onpty3": false,
    "pty3_account": null,
    "label_provided": false,
    "tracking_number": null,
    "client_po": null,
    "status": 1,
    "order_state_id": 1,
    "picking_method_id": 2,
    "processing_type_id": 3,
    "internal_order": "1-186-B",
    "warehouse_name": "3DM-AVRO",
    "updated_at": "2024-03-06T19:57:48.000000Z",
    "created_at": "2024-03-06T19:57:48.000000Z",
    "id": 6157,
    "order_items": [
      {
        "id": 2701,
        "order_id": 6157,
        "item_id": 6439,
        "descriptions": "",
        "quantity_ordered": 1,
        "sku": "aipods2",
        "lot": "",
        "expiry_date": null,
        "order_item_status_id": 3,
        "created_by": "Genming Zhao",
        "created_at": "2024-03-06T19:57:48.000000Z",
        "uom_type_id": 1,
        "sale_price": "7.00",
        "sent_serial_number_on": null,
        "quantity_shipped": 0,
        "kit": null,
        "kit_type": null,
        "uom_quantity": 1,
        "quantity_each": 1,
        "quantity_reserved": 0,
        "quantity_backorder": 0,
        "quantity_allocated": 0,
        "quantity_processed": 0,
        "quantity_picked": 0,
        "quantity_packed": 0
      }
    ]
  }
}
```
