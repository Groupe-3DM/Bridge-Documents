# Retrieve return labels

### URL

```text
api/v1/admin/return-labels/:id
```

### Method

```text
GET
```

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