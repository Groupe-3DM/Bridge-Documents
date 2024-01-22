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

| Name            | Type    | Required | Default | Description |
|-----------------|---------|----------|---------|-------------|
| tracking_number | string  | yes      |         | max<199     |
| order_id        | integer | yes      |         |             |
| carrier_id      | integer | yes      |         |             |
| label_url       | string  | yes      |         | max<255     |

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
    "order_id":1,
    "carrier_id":1,
    "tracking_number":"333333",
    "label_url":"dateste"

}
```

### Success response

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "id": 1,
    "order_id": 26,
    "carrier_id": 1,
    "tracking_number": "333333",
    "label_url": "dateste",
    "created_by": "Genming gggg",
    "updated_by": "Genming gggg"
  }
}
```