# Retrieve orders history

### URL

```text
api/v1/statistics/orders/history
```

### Method

```text
GET
```

### Parameters

| Name       | Type    | Required | Default | Description                                                                    |
|------------|---------|----------|---------|--------------------------------------------------------------------------------|
| start_date | date    | Yes      |         | Y-m-d    <br/>after:2023-04-07                                                 |
| end_date   | date    | Yes      |         | Y-m-d    <br/>after_or_equal:start_date<br>before:tomorrow <br/>max:1(365)year |
| client_id  | integer |          |         |                                                                                |
| date_field | string  | Yes      |         | "order_date","process_date","shipped_date"                                     |

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
    "2023-12-01": 0,
    "2023-12-02": 0,
    "2023-12-03": 0,
    "2023-12-04": 0,
    "2023-12-05": 0,
    "2023-12-06": 0,
    "2023-12-07": 0,
    "2023-12-08": 0,
    "2023-12-09": 0,
    "2023-12-10": 0,
    "2023-12-11": 0,
    "2023-12-12": 0,
    "2023-12-13": 0,
    "2023-12-14": 0,
    "2023-12-15": 0,
    "2023-12-16": 0,
    "2023-12-17": 0,
    "2023-12-18": 0,
    "2023-12-19": 0,
    "2023-12-20": 9,
    "2023-12-21": 2,
    "2023-12-22": 0,
    "2023-12-23": 0,
    "2023-12-24": 0,
    "2023-12-25": 0,
    "2023-12-26": 0,
    "2023-12-27": 0,
    "2023-12-28": 0,
    "2023-12-29": 0
  }
}

```