# Retrieve a list of orders with query builder

### URL

```text
api/v1/orders
```

### Method

```text
GET
```

### Parameters

| Name            | Type         | Required | Default | Description                                                  |
|-----------------|--------------|----------|---------|--------------------------------------------------------------|
| order_number    | string       |          |         |                                                              |
| client_id       | id/array     |          |         |                                                              |
| sku             | string/array |          |         |                                                              |
| first_name      | string       |          |         |                                                              |
| last_name       | string       |          |         |                                                              |
| telephone       | string       |          |         |                                                              |
| email           | string       |          |         |                                                              |
| company         | string       |          |         |                                                              |
| date_field      | string       |          |         | shipped_date/order_date/process_date                         |
| start_date      | Date         |          |         |                                                              |
| end_date        | Date         |          |         |                                                              |
| order_from      | date         |          |         |                                                              |
| order_to        | Date         |          |         |                                                              |
| arrival_from    | Date         |          |         |                                                              |
| arrival_to      | Date         |          |         |                                                              |
| postal_code     | string       |          |         |                                                              |
| country_id      | id           |          |         | [APIs](../Others/get_countries.md)                           |
| province_id     | id           |          |         | [APIs](../Others/get_provinces.md)                           |
| order_status_id | Id           |          |         | [APIs](../Others/get_order_statuses.md)                      |
| order_state_id  | Id           |          |         | [APIs](../Others/get_order_states.md)                        |
| ready           | boolean      |          |         |                                                              |
| processing_type | number       |          |         |                                                              |
| sort_by         | string       |          |         | any of above field                                           |
| sort_order      | string       |          |         | DESC/ASC                                                     |
| limit           | integer      |          |         | <200                                                         |
| list            | string       |          |         | all/first/last/count/take/auto-complete (default: paginated) |

### Note

```text
* query's example: date_field=shipped_date&start_date=2023-09-10&end_date=2023-09-20&limit=20&list=all

* paginated data will give out if no flag of list
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
    "id": 242,
    "client_id": 9999,
    "order_number": "1041",
    "order_date": "2023-03-22 11:47:53",
    "order_state_id": 1,
    "order_status_id": 17,
    "order_type_id": null,
    "processing_type_id": null,
    "parent_id": null,
    "first_name": "test",
    "last_name": "etst",
    "email": "",
    "company": "",
    "telephone": "",
    "address1": "328 Rue Avro",
    "address2": "",
    "address3": null,
    "postal_code": "H9R 5W5",
    "apt_num1": null,
    "apt_num2": null,
    "city": "Pointe-Claire",
    "province_id": 612,
    "country_id": 38,
    "reference1": null,
    "reference2": null,
    "packing_slip_note": null,
    "pick_up": 0,
    "inside_delivery": 0,
    "lift_gate_required": 0,
    "ready": 1,
    "is_master": 0,
    "process_date": null,
    "deliver_by_date": null,
    "handling_priority": 0,
    "processing_priority": 0,
    "temperature_control": null,
    "hazmat": 0,
    "appointment_required": 0,
    "order_handling": 0,
    "signature_required": 0,
    "ambient_control": 0,
    "air_ground_control": 0,
    "handling_instruction": null,
    "dangerous_goods": 0,
    "language_id": null,
    "carrier_id": null,
    "service_id": null,
    "packing_slips": null,
    "note": null,
    "custom_reference_no": null,
    "label_provided": 0,
    "shipping_label_file": null,
    "client_order_id": "5105233264835",
    "trackings": null,
    "client_name": "TEST",
    "order_items": [
      {
        "id": 427,
        "order_id": 242,
        "item_id": 4273,
        "descriptions": "New test sku 1",
        "quantity_ordered": 1,
        "sku": "NewTestSku1",
        "lot": "",
        "expiry_date": null,
        "unit_value": "0.0000",
        "order_item_status_id": 1,
        "uom_type_id": 1,
        "created_by": null,
        "created_at": "2023-05-11T15:00:53.000000Z",
        "sale_price": "0.00"
      },
      {
        "id": 428,
        "order_id": 242,
        "item_id": 4274,
        "descriptions": "New test sku 2",
        "quantity_ordered": 1,
        "sku": "NewTestSku2",
        "lot": "",
        "expiry_date": null,
        "unit_value": "0.0000",
        "order_item_status_id": 1,
        "uom_type_id": 1,
        "created_by": null,
        "created_at": "2023-05-11T15:00:53.000000Z",
        "sale_price": "0.00"
      }
    ]
  }
}
```