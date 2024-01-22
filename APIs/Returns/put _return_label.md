# Retrieve return labels

### URL

```text
api/v1/admin/return-labels/:id
```

### Method

```text
PUT
```

### Parameters

| Name            | Type    | Required | Default | Description |
|-----------------|---------|----------|---------|-------------|
| tracking_number | string  |          |         | max<199     |
| order_id        | integer |          |         |             |
| carrier_id      | integer |          |         |             |
| label_url       | string  |          |         | max<255     |

### Note

```text

```

### Auth required (Admin)

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
  
    "tracking_number":"333999333"
   

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
    "tracking_number": "333999333",
    "label_url": "dateste",
    "created_by": "Genming gggg",
    "updated_by": "Genming gggg"
  }
}
```