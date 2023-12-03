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
| order_number | string  |          |         |                                              |
| order_id     | integer |          |         |                                              |
| client_id    | integer |          |         |                                              |
| date_field   | string  |          |         | created_at/ship_date/estimated_delivery_date |
| start_date   | date    |          |         |                                              |
| end_date     | date    |          |         |                                              |
| sort_by      | string  |          |         | any of above field                           |
| sort_order   | string  |          |         | DESC/ASC                                     |
| limit        | integer |          | 15      | max<200                                      |
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
            "expiry_date": null
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
            "expiry_date": null
          }
        ]
      },
      {
        "id": 2,
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
        "client_id": null,
        "client_name": null,
        "order_package_items": []
      },
      {
        "id": 3,
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
        "client_id": null,
        "client_name": null,
        "order_package_items": []
      },
      {
        "id": 4,
        "order_id": 348,
        "tracking": "1Z001985YW99744790",
        "tracking_url": "https://www.ups.com/WebTracking?loc=en_US&requester=ST&trackNums=1Z001985YW99744790",
        "carrier": "UPS",
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
        "carrier_id": 1,
        "order_number": "33-12-6-2",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": []
      },
      {
        "id": 5,
        "order_id": 348,
        "tracking": "1234",
        "tracking_url": "https://www.ups.com/WebTracking?loc=en_US&requester=ST&trackNums=1Z001985YW99744790",
        "carrier": "UPS",
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
        "carrier_id": 1,
        "order_number": "33-12-6-2",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": []
      },
      {
        "id": 6,
        "order_id": 242,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1041",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": []
      },
      {
        "id": 7,
        "order_id": 243,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1043",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": [
          {
            "id": 3,
            "order_item_id": 429,
            "order_id": 243,
            "item_id": 4273,
            "order_package_id": 7,
            "quantity": 1,
            "description": null,
            "sku": "NewTestSku1",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          },
          {
            "id": 4,
            "order_item_id": 430,
            "order_id": 243,
            "item_id": 4274,
            "order_package_id": 7,
            "quantity": 1,
            "description": null,
            "sku": "NewTestSku2",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          }
        ]
      },
      {
        "id": 8,
        "order_id": 244,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1044",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": [
          {
            "id": 5,
            "order_item_id": 431,
            "order_id": 244,
            "item_id": 4274,
            "order_package_id": 8,
            "quantity": 1,
            "description": null,
            "sku": "NewTestSku2",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          },
          {
            "id": 6,
            "order_item_id": 432,
            "order_id": 244,
            "item_id": 4273,
            "order_package_id": 8,
            "quantity": 1,
            "description": null,
            "sku": "NewTestSku1",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          }
        ]
      },
      {
        "id": 9,
        "order_id": 245,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1048",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": [
          {
            "id": 7,
            "order_item_id": 433,
            "order_id": 245,
            "item_id": 4270,
            "order_package_id": 9,
            "quantity": 1,
            "description": null,
            "sku": "YESTESTSKU",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          }
        ]
      },
      {
        "id": 10,
        "order_id": 246,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1049",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": [
          {
            "id": 8,
            "order_item_id": 434,
            "order_id": 246,
            "item_id": 4270,
            "order_package_id": 10,
            "quantity": 2,
            "description": null,
            "sku": "YESTESTSKU",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          },
          {
            "id": 9,
            "order_item_id": 435,
            "order_id": 246,
            "item_id": 4271,
            "order_package_id": 10,
            "quantity": 1,
            "description": null,
            "sku": "ITP123",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          }
        ]
      },
      {
        "id": 11,
        "order_id": 247,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1050",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": [
          {
            "id": 10,
            "order_item_id": 436,
            "order_id": 247,
            "item_id": 4270,
            "order_package_id": 11,
            "quantity": 2,
            "description": null,
            "sku": "YESTESTSKU",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          }
        ]
      },
      {
        "id": 12,
        "order_id": 248,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1051",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": [
          {
            "id": 11,
            "order_item_id": 437,
            "order_id": 248,
            "item_id": 4270,
            "order_package_id": 12,
            "quantity": 4,
            "description": null,
            "sku": "YESTESTSKU",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          }
        ]
      },
      {
        "id": 13,
        "order_id": 249,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1052",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": [
          {
            "id": 12,
            "order_item_id": 438,
            "order_id": 249,
            "item_id": 4270,
            "order_package_id": 13,
            "quantity": 4,
            "description": null,
            "sku": "YESTESTSKU",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          }
        ]
      },
      {
        "id": 14,
        "order_id": 250,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1053",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": [
          {
            "id": 13,
            "order_item_id": 439,
            "order_id": 250,
            "item_id": 4270,
            "order_package_id": 14,
            "quantity": 2,
            "description": null,
            "sku": "YESTESTSKU",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          }
        ]
      },
      {
        "id": 15,
        "order_id": 251,
        "tracking": null,
        "tracking_url": null,
        "carrier": null,
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
        "order_number": "1058",
        "order_package_status_id": 5,
        "client_id": null,
        "client_name": null,
        "order_package_items": [
          {
            "id": 14,
            "order_item_id": 440,
            "order_id": 251,
            "item_id": 4270,
            "order_package_id": 15,
            "quantity": 1,
            "description": null,
            "sku": "YESTESTSKU",
            "serial_number": null,
            "lot": null,
            "expiry_date": null
          }
        ]
      }
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