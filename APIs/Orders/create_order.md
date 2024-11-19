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

| Name                           | Type        | Required                 | Default | Description                        |
|--------------------------------|-------------|--------------------------|---------|------------------------------------|
| client_id                      | id          | Y                        |         |                                    |
| order_number                   | string      |                          |         |                                    |
| order_date                     | Y-m-d H:i:s | Y                        |         |                                    |
| first_name                     | string      | Y                        |         |                                    |
| last_name                      | string      |                          |         |                                    |
| apt_num1                       | string      |                          |         |                                    |
| apt_num2                       | string      |                          |         |                                    |
| address1                       | string      | Y                        |         | max 35 characters                  |
| address2                       | string      |                          |         | max 35 characters                  |
| city                           | string      | Y                        |         |                                    |
| province_id                    | id/code     | Y                        |         | [APIs](../Others/get_provinces.md) |
| country_id                     | id/iso2     | Y                        |         | [APIs](../Others/get_countries.md) |
| company                        | string      |                          |         |                                    |
| telephone                      | string      |                          |         |                                    |
| email                          | string      |                          |         |                                    |
| postal_code                    | string      | Y                        |         |                                    |
| reference1                     | string      |                          |         |                                    |
| reference2                     | string      |                          |         |                                    |
| note                           | string      |                          |         |                                    |
| custom_reference_no            | string      |                          |         |                                    |
| packing_slip_note              | string      |                          |         |                                    |
| order_items                    | array       | Y                        |         |                                    |
| order_items.*                  | array       | Y                        |         |                                    |
| order_items.*.quantity_ordered | integer     | Y                        |         |                                    |
| order_items.*.uom_type_id      | id          | Y                        |         | [APIs](../Others/get_uom_types.md) |
| order_items.*.item_id          | id          |                          |         | [APIs](../Products/get_items.md)   |
| order_items.*.sku              | string      | Y if item_id not present |         |                                    |
| order_items.*.lot              | string      |                          |         |                                    |
| order_items.*.expiry_date      | date        |                          |         |                                    |
| order_items.*.line_number      | string      |                          |         |                                    |
| order_items.*.sale_price       | decimal     |                          |         | unit value                         |

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
  "province_id": "qc",
  "country_id": "CA",
  "city": "Montreal",
  "postal_code": "H9R 3S4",
  "order_items": [
    {
      "sku": "aipods2",
      "quantity_ordered": 1,
      "uom_type_id": 1,
      "line_number": 4
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
    "order_number": 1709774153,
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
    "apt_num1": null,
    "apt_num2": null,
    "reference1": null,
    "reference2": null,
    "packing_slip_note": null,
    "order_status_id": 1,
    "note": null,
    "custom_reference_no": null,
    "created_by": "xxxx",
    "updated_by": "xxxx",
    "status": 1,
    "order_state_id": 1,
    "updated_at": "2024-03-06 20:15:54",
    "created_at": "2024-03-06 20:15:54",
    "id": 6248,
    "order_items": [
      {
        "id": 2709,
        "order_id": 6248,
        "item_id": 6439,
        "descriptions": null,
        "quantity_ordered": 1,
        "sku": "aipods2",
        "lot": null,
        "expiry_date": null,
        "uom_type_id": 1,
        "line_number": "4"
      }
    ]
  }
}
```
