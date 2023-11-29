# Create an order

`endpoint: api/v1/orders`

`Method: POST`


### Parameters

| Name                           | Type    | Mandatory |
|--------------------------------|---------|-----------|
| client_id                      | integer | Y         |
| order_number                   | string  |           |
| order_date                     | string  | Y         |
| first_name                     | string  | Y         |
| last_name                      | string  |           |
| apt_num1                       | string  |           |
| apt_num2                       | string  |           |
| address1                       | string  | Y         |
| address2                       | string  |           |
| city                           | string  | Y         |
| province_id                    | string  | Y         |
| country_id                     | string  | Y         |
| company                        | string  |           |
| telephone                      | string  |           |
| email                          | string  |           |
| postal_code                    | string  | Y         |
| reference1                     | string  |           |
| reference2                     | string  |           |
| packing_slip_note              | string  |           |
| pick_up                        | boolean |           |
| lift_gate_required             | boolean |           |
| processing_priority            | boolean |           |
| handling_priority              | boolean |           |
| hazmat                         | boolean |           |
| appointment_required           | boolean |           |
| dangerous_goods                | boolean |           |
| carrier_id                     | integer |           |
| service_id                     | integer |           |
| note                           | string  |           |
| custom_reference_no            | string  |           |
| deliver_by_date                | date    |           |
| signature_required             | boolean |           |
| ambient_control                | boolean |           |
| air_ground_control             | boolean |           |
| order_items                    | array   | Y         |
| order_items.*                  | array   | Y         |
| order_items.*.quantity_ordered | integer | Y         |
| order_items.*.uom_quantity_id  | integer | Y         |
| order_items.*.item_id          | integer | Y         |
| order_items.*.lot              | integer |           |
| order_items.*.expiry_date      | date    |           |
| order_items.*.unit_value       | integer |           |


# Response:
```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "client_id": 1,
    "order_number": 1689625979,
    "order_date": "2023-09-09 11:11:11",
    "email": null,
    "first_name": "jon",
    "last_name": null,
    "address1": "222 ave mntril",
    "province_id": 121,
    "country_id": 38,
    "city": "kkkkkkk",
    "telephone": null,
    "company": null,
    "postal_code": "kkkk",
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
    "order_status_id": 15,
    "pick_up": false,
    "inside_delivery": false,
    "lift_gate_required": false,
    "hazmat": false,
    "order_handling": false,
    "appointment_required": false,
    "temperature_control": false,
    "dangerous_goods": false,
    "language_id": 1,
    "warehouse_id": 12,
    "carrier_id": null,
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
    "picking_method_id": 1,
    "processing_type_id": 2,
    "internal_order": "1-18",
    "updated_at": "2023-07-17T20:32:59.000000Z",
    "created_at": "2023-07-17T20:32:59.000000Z",
    "id": 341,
    "warehouse_name": "3DM - AVRO",
    "client_name": "Group 3-DM",
    "order_items": [
      {
        "id": 583,
        "order_id": 341,
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
        "created_at": "2023-07-17T20:32:59.000000Z",
        "sale_price": "3.00"
      }
    ]
  }
}
```