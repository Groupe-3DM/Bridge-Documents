# Retrieve orders information

### URL

```text
api/v1/statistics/orders/information
```

### Method

```text
GET
```

### Parameters

| Name       | Type    | Required | Default | Description |
|------------|---------|----------|---------|-------------|
| start_date | date    | Yes      |         | Y-m-d       |
| end_date   | date    | Yes      |         | Y-m-d       |
| client_id  | integer |          |         |             |

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

```

### Success response

```json

{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "create": 11,
    "process": 0,
    "ship": 0
  }
}

```