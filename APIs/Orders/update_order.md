# Update an order

### URL

```text
api/v1/orders/:id
```

### Method

```text
PUT
```

### Parameters

| Name                           | Type    | Required                           | Default | Description                        |
|--------------------------------|---------|------------------------------------|---------|------------------------------------|
| client_id                      | integer |                                    |         | [APIs](../Clients/get_clients.md)  |
| order_number                   | string  |                                    |         |                                    |
| order_date                     | string  |                                    |         |                                    |
| first_name                     | string  |                                    |         |                                    |
| last_name                      | string  |                                    |         |                                    |
| apt_num1                       | string  |                                    |         |                                    |
| apt_num2                       | string  |                                    |         |                                    |
| address1                       | string  |                                    |         | max 35 characters                  |
| address2                       | string  |                                    |         | max 35 characters                  |
| city                           | string  |                                    |         |                                    |
| province_id                    | integer |                                    |         | [APIs](../Others/get_provinces.md) |
| country_id                     | integer |                                    |         | [APIs](../Others/get_countries.md) |
| company                        | string  |                                    |         |                                    |
| telephone                      | string  |                                    |         |                                    |
| email                          | email   |                                    |         |                                    |
| postal_code                    | string  |                                    |         |                                    |
| reference1                     | string  |                                    |         |                                    |
| reference2                     | string  |                                    |         |                                    |
| note                           | string  |                                    |         |                                    |
| custom_reference_no            | string  |                                    |         |                                    |
| packing_slip_note              | string  |                                    |         |                                    |
| order_items                    | array   |                                    |         |                                    |
| order_items.*                  | array   | Y if order_items exists in payload |         |                                    |
| order_items.*.quantity_ordered | integer | Y if order_items exists in payload |         |                                    |
| order_items.*.uom_quantity_id  | integer | Y if order_items exists in payload |         | [APIs](../Others/get_uom_types.md) |
| order_items.*.lot              | string  |                                    |         |                                    |
| order_items.*.expiry_date      | date    |                                    |         |                                    |
| order_items.*.unit_value       | integer |                                    |         |                                    |

### Note

```text
* updating order is available if  order_status id in (14 receiving , 1 received, 2 released, 12 backorder)
* master order can't be updated once it created
* any updating execution could lead to the creation of backorder
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
  "order_number": "1689625979",
  "order_date": "2023-09-09 11:11:11",
  "email": "test@email.com",
  "first_name": "john",
  "last_name": "Don",
  "address1": "222 ave mntril",
  "address2": "",
  "province_id": 612,
  "country_id": 38,
  "city": "Montreal",
  "telephone": null,
  "company": null,
  "postal_code": "H9R 3S4",
  "note": null,
  "custom_reference_no": null,
  "client_po": null,
  "reference1": null,
  "reference2": null,
  "order_items": [
    {
      "item_id": 1,
      "quantity_ordered": 1,
      "lot": "",
      "expiry_date": null,
      "unit_value": "0.0000",
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
    "id": 336,
    "client_id": 1,
    "order_number": "1688736219",
    "internal_order": "1-13",
    "order_date": "2023-09-09 11:11:11",
    "status": 1,
    "order_status_id": 1,
    "order_type_id": 1,
    "processing_type_id": 2,
    "parent_id": null,
    "first_name": "j",
    "last_name": null,
    "email": null,
    "company": null,
    "telephone": null,
    "address1": "111",
    "address2": null,
    "address3": null,
    "postal_code": "kkkk",
    "apt_num1": null,
    "apt_num2": null,
    "city": "kkkkkkk",
    "province_id": 121,
    "country_id": 38,
    "reference1": null,
    "reference2": null,
    "packing_slip_note": null,
    "pick_up": 0,
    "inside_delivery": 0,
    "lift_gate_required": 0,
    "ready": 0,
    "is_master": 0,
    "process_date": null,
    "deliver_by_date": null,
    "handling_priority": 0,
    "processing_priority": 0,
    "temperature_control": 0,
    "hazmat": 0,
    "appointment_required": 0,
    "order_handling": 0,
    "signature_required": 0,
    "ambient_control": 0,
    "air_ground_control": 0,
    "handling_instruction": null,
    "dangerous_goods": 0,
    "language_id": 1,
    "carrier_id": null,
    "service_id": null,
    "packing_slips": null,
    "note": null,
    "custom_reference_no": null,
    "label_provided": 0,
    "shipping_label_file": null,
    "client_order_id": null,
    "trackings": null,
    "client_name": "Group 3-DM",
    "order_items": [
      {
        "id": 579,
        "order_id": 336,
        "item_id": 1,
        "descriptions": "",
        "quantity_ordered": 1,
        "sku": "sku1236",
        "lot": "",
        "expiry_date": null,
        "unit_value": "0.0000",
        "order_item_status_id": 1,
        "uom_type_id": 1,
        "created_by": "Genming Zhao",
        "created_at": "2023-07-16T19:23:20.000000Z",
        "sale_price": "3.00"
      }
    ]
  }
}
```

