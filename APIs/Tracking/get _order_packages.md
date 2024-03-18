# Retrieve order tracking information

### URL

```text
api/v1/order-packages
```

### Method

```text
GET
```

### Parameters

| Name         | Type    | Required | Default | Description                                  |
|--------------|---------|----------|---------|----------------------------------------------|
| order_number | string  |          |         | ex: xxxx1,xxx2,xxx3                          |
| order_id     | id      |          |         |                                              |
| client_id    | id      |          |         |                                              |
| date_field   | string  |          |         | created_at/ship_date/estimated_delivery_date |
| start_date   | date    |          |         |                                              |
| end_date     | date    |          |         |                                              |
| sort_by      | string  |          |         | any of above field                           |
| sort_order   | string  |          |         | DESC/ASC                                     |
| limit        | integer |          | 15      | max<500                                      |
| list         | string  |          |         | all/count/take/auto-complete                 |

### Note

```text
* query's example: date_field=ship_date&start_date=2023-09-10&end_date=2023-09-20&limit=20&list=all

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
    "data": [
      {
        "id": 1,
        "order_id": 226,
        "tracking": "asdfsdfsdfsd",
        "tracking_url": "",
        "carrier": "test",
        "delivery_service": null,
        "price": null,
        "label_id": null,
        "label_path": null,
        "label_format": null,
        "estimated_delivery_date": null,
        "possible_pickup_date": null,
        "currency": null,
        "ship_date": null,
        "length": "0.00",
        "width": "0.00",
        "height": "0.00",
        "weight": "0.00",
        "package_description": null,
        "warehouse_id": null,
        "carrier_id": null,
        "order_number": "33-12-6-2",
        "order_package_status_id": 5,
        "client_id": 1,
        "client_name": null,
        "order_package_items": [
          {
            "id": 1,
            "order_item_id": 427,
            "order_id": 242,
            "item_id": 4273,
            "order_package_id": 1,
            "quantity": 1,
            "description": null,
            "sku": "NewTestSku1",
            "serial_number": null,
            "lot": null,
            "expiry_date": null,
            "line_number": "xxx"
          },
          {
            "id": 2,
            "order_item_id": 428,
            "order_id": 242,
            "item_id": 4274,
            "order_package_id": 1,
            "quantity": 1,
            "description": null,
            "sku": "NewTestSku2",
            "serial_number": null,
            "lot": null,
            "expiry_date": null,
            "line_number": null
          }
        ]
      },
      
    ],
    "current_page": 1,
    "last_page": 3,
    "from": 1,
    "to": 15,
    "total": 38,
    "per_page": 15
  }
}
```
