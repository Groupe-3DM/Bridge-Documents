# Update an order

### URL

```text
api/v1/orders/update/address
```

### Method

```text
POST
```

### Parameters

| Name         | Type         | Required         | Default | Description                        |
|--------------|--------------|------------------|---------|------------------------------------|
| client_id    | id           | Y                |         |                                    |
| order_id     | id           |                  |         |                                    |
| order_number | string       | Y if no order_id |         |                                    |
| first_name   | string       |                  |         |                                    |
| last_name    | string       |                  |         |                                    |
| apt_num1     | string       |                  |         |                                    |
| apt_num2     | string       |                  |         |                                    |
| address1     | string       |                  |         | max 35 characters                  |
| address2     | string       |                  |         | max 35 characters                  |
| city         | string       |                  |         |                                    |
| province_id  | id/code      |                  |         | [APIs](../Others/get_provinces.md) |
| country_id   | id/iso2/iso3 |                  |         | [APIs](../Others/get_countries.md) |
| company      | string       |                  |         |                                    |
| telephone    | string       |                  |         |                                    |
| email        | email        |                  |         |                                    |
| postal_code  | string       |                  |         |                                    |

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
  "client_id": 1,
  "order_number": "1689625979",
  "email": "test@email.com",
  "first_name": "john",
  "last_name": "Don",
  "address1": "222 ave mntril",
  "address2": "",
  "province_id": "QC",
  "country_id": "CA",
  "city": "Montreal"
}
```

### Success response

```json
{
  "success": true,
  "message": "Action has been successfully processed(47)",
  "data": true
}
```

