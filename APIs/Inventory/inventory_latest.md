# Latest modified Inventory

### URL
```text
api/v1/inventory/item/latest-modified
```

### Method
```text
GET
```

### Parameters

| Name      | Type    | Required | Default | Description |
|-----------|---------|----------|---------|-------------|
| client_id | integer | Y        |

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
      "qty": 1026
    }
  ]
}
```