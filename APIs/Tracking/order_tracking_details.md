# Retrieve order tracking information


`endpoint: api/v1/order-packages/order/details`
`method: GET`

### Parameters

------------------------------------------------------------------

| Name         | Type   |
|--------------|--------|
| order_number | string |
| client_id    | index  |

### Response

--------------------------------------------------------------

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
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
    }
  ]
}
```

`endpoint: api/v1/orders/shipment/cost-estimated`
`method: GET`

### Parameters

------------------------------------------------------------------

| Name         | Type   |
|--------------|--------|
| order_number | string |

### Response

--------------------------------------------------------------

```json

```

----------------------------------------------------------------
`endpoint: api/v1/orders/shipment/cost`
`method: GET`

### Parameters

------------------------------------------------------------------

| Name         | Type   |
|--------------|--------|
| order_number | string |

### Response

--------------------------------------------------------------

```json

```