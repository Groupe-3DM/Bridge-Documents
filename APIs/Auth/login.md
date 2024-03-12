# Login to retrieve authenticated user's information

### URL

```text
api/v1/login
```

### Method

```text
POST
```

### Parameters


| Name     | Type   | Required | Default | Description |
|----------|--------|----------|---------|-------------|
| email    | email  | Y        |         |             |
| password | string | Y        |         |             |

### Auth required
```text
NO
```


### Headers
```text
Content-Type: application/json
Accept: application/json

```



### Request example

```json
{
  "email": "your-email@domain.com",
  "password": "xxxxxxx"
}
```

### Success example

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "token":"xxxx",
    "name": "xxxxxx",
    "user": {
      "id": 2,
      "first_name": "xxxxx",
      "last_name": "xxx",
      "email": "test@3-dm.com",
      "home_phone": "514-123-1234",
      "cell_phone": "514-123-1234",
      "office_phone": "514-123-1234",
      "office_extension": "514-123-1234",
      "notifying": 1,
      "address1": "514-123-1234",
      "address2": null,
      "postal_code": "h9r5x7",
      "city": "montreal",
      "province_id": 612,
      "country_id": 38,
      "language_id": 2,
      "status": 1,
      "notes": "test",
      "order_error": 1,
      "item_error": 1,
      "permissions": [
        {
          "id": 1,
          "name": "xxxxxx",
          "internal": 1,
          "external": 1,
          "parent_id": null
        }
      ],
      "clients": [
        6070,
        1,
        10000,
        10001
      ],
      "roles": [
        11
      ]
    }
  }
}
```