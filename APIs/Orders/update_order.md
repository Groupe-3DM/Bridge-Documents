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

| Name                           | Type    | Required                           | Default | description |
|--------------------------------|---------|------------------------------------|---------|-------------|
| client_id                      | integer |                                    |         |             |
| order_number                   | string  |                                    |         |             |
| order_date                     | string  |                                    |         |             |
| first_name                     | string  |                                    |         |             |
| last_name                      | string  |                                    |         |             |
| apt_num1                       | string  |                                    |         |             |
| apt_num2                       | string  |                                    |         |             |
| address1                       | string  |                                    |         |             |
| address2                       | string  |                                    |         |             |
| city                           | string  |                                    |         |             |
| province_id                    | string  |                                    |         |             |
| country_id                     | string  |                                    |         |             |
| company                        | string  |                                    |         |             |
| telephone                      | string  |                                    |         |             |
| email                          | string  |                                    |         |             |
| postal_code                    | string  |                                    |         |             |
| reference1                     | string  |                                    |         |             |
| reference2                     | string  |                                    |         |             |
| packing_slip_note              | string  |                                    |         |             |
| pick_up                        | boolean |                                    |         |             |
| lift_gate_required             | boolean |                                    |         |             |
| processing_priority            | boolean |                                    |         |             |
| handling_priority              | boolean |                                    |         |             |
| hazmat                         | boolean |                                    |         |             |
| appointment_required           | boolean |                                    |         |             |
| dangerous_goods                | boolean |                                    |         |             |
| carrier_id                     | integer |                                    |         |             |
| service_id                     | integer |                                    |         |             |
| note                           | string  |                                    |         |             |
| custom_reference_no            | string  |                                    |         |             |
| deliver_by_date                | date    |                                    |         |             |
| signature_required             | boolean |                                    |         |             |
| ambient_control                | boolean |                                    |         |             |
| air_ground_control             | boolean |                                    |         |             |
| order_items                    | array   |                                    |         |             |
| order_items.*                  | array   | Y if order_items exists in payload |         |             |
| order_items.*.quantity_ordered | integer | same as above                      |         |             |
| order_items.*.uom_quantity_id  | integer | same as above                      |         |             |
| order_items.*.item_id          | integer | same as above                      |         |             |
| order_items.*.lot              | integer |                                    |         |             |
| order_items.*.expiry_date      | date    |                                    |         |             |
| order_items.*.unit_value       | integer |                                    |         |             |



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

