# inventory info of sku

### URL

```text
api/v1/inventories/item/info
```

### Method

```text
GET
```

### Parameters

| Name             | Type    | Required | Default | Description                                                                                |
|------------------|---------|----------|---------|--------------------------------------------------------------------------------------------|
| client_id        | integer | Y        |         |                                                                                            |
| quantity_type_id | integer | Y        |         | 1 available 2 reserved 3 receiving 4 allocated 5 damaged 6 quarantine 7 returned 8 expired |

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

### Success Response
```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": [
    {
      "sku": "sku1236",
      "item_id": 1,
      "client_id": "1",
      "qty": 1078
    },
    {
      "sku": "",
      "item_id": 11,
      "client_id": "1",
      "qty": 1993
    },
    {
      "sku": "JIF-321",
      "item_id": 2,
      "client_id": "1",
      "qty": 1061
    },
    {
      "sku": "b-12-12",
      "item_id": 4,
      "client_id": "1",
      "qty": 264
    },
    {
      "sku": "JIF-ABC",
      "item_id": 3,
      "client_id": "1",
      "qty": 28
    },
    {
      "sku": "yu67",
      "item_id": 2,
      "client_id": "1",
      "qty": 100
    },
    {
      "sku": "SKU123sdf",
      "item_id": 2514,
      "client_id": "1",
      "qty": 1000
    },
    {
      "sku": 73000,
      "item_id": 1,
      "client_id": "1",
      "qty": 3
    }
  ]
}
```