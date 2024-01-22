# Retrieve return labels

### URL

```text
api/v1/admin/return-labels
```

### Method

```text
GET
```

### Parameters

| Name            | Type    | Required | Default | Description                                  |
|-----------------|---------|----------|---------|----------------------------------------------|
| tracking_number | string  |          |         |                                              |
| order_id        | integer |          |         |                                              |
| carrier_id      | integer |          |         |                                              |
| sort_order      | string  |          |         | DESC/ASC                                     |
| limit           | integer |          | 15      | max<200                                      |
| list            | string  |          |         | all/count/take/auto-complete                 |

### Note

```text


* paginated data will give out if no flag of list
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
    "current_page": 1,
    "data": [
      {
        "id": 1,
        "order_id": 26,
        "carrier_id": 1,
        "tracking_number": "339993333",
        "label_url": "dateste",
        "created_by": "Genming gggg",
        "updated_by": "Genming gggg"
      }
    ],
    "from": 1,
    "last_page": 1,
    "per_page": 15,
    "to": 1,
    "total": 1
  }
}
```