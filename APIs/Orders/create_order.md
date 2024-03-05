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

| Name                           | Type    | Required | Default | Description                        |
|--------------------------------|---------|----------|---------|------------------------------------|
| client_id                      | integer | Y        |         | [APIs](../Clients/get_clients.md)  |
| order_number                   | string  |          |         |                                    |
| order_date                     | string  | Y        |         |                                    |
| first_name                     | string  | Y        |         |                                    |
| last_name                      | string  |          |         |                                    |
| apt_num1                       | string  |          |         |                                    |
| apt_num2                       | string  |          |         |                                    |
| address1                       | string  | Y        |         |                                    |
| address2                       | string  |          |         |                                    |
| city                           | string  | Y        |         |                                    |
| province_id                    | integer | Y        |         | [APIs](../Others/get_provinces.md) |
| country_id                     | integer | Y        |         | [APIs](../Others/get_countries.md) |
| company                        | string  |          |         |                                    |
| telephone                      | string  |          |         |                                    |
| email                          | email   |          |         |                                    |
| postal_code                    | string  | Y        |         |                                    |
| reference1                     | string  |          |         |                                    |
| reference2                     | string  |          |         |                                    |
| note                           | string  |          |         |                                    |
| custom_reference_no            | string  |          |         |                                    |
| packing_slip_note              | string  |          |         |                                    |
| order_items                    | array   | Y        |         |                                    |
| order_items.*                  | array   | Y        |         |                                    |
| order_items.*.quantity_ordered | integer | Y        |         |                                    |
| order_items.*.uom_quantity_id  | integer | Y        |         | [APIs](../Others/get_uom_types.md) |
| order_items.*.item_id          | integer | Y        |         | [APIs](../Products/get_items.md)   |
| order_items.*.lot              | integer |          |         |                                    |
| order_items.*.expiry_date      | date    |          |         |                                    |
| order_items.*.unit_value       | integer |          |         |                                    |


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
    "id": 341,
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
    "carrier_id": null,
    "service_id": null,
    "note": null,
    "custom_reference_no": null,
    "created_by": "Genming Zhao",
    "updated_by": "Genming Zhao",
    "deliver_by_date": null,
    "signature_required": false,
    "ambient_control": false,
    "air_ground_control": 0,
    "label_provided": false,
    "client_po": null,
    "status": 1,
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
