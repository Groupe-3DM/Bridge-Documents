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
| tracking_number | string  |          |         | max<199     |
| order_id        | integer |          |         |             |
| carrier_id      | integer |          |         |             |
| label_url       | string  |          |         | max<255     |

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