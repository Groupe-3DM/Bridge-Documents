# Verify authenticated user's information


### URL
```text
api/v1/me
```

### Method
```text
GET
```

### Parameters

| Name     | Type   | Required | Default | Description |
|----------|--------|----------|---------|-------------|


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

### Success example

```json
{
    "success": true,
    "message": "Operation has been successfully completed!",
    "data": {
        "id": 2,
        "first_name": "aaaa",
        "last_name": "gggg",
        "email": "XXX@email.com",
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
        "warehouse_id": 1,
        "status": 1,
        "department_id": 1,
        "employee": 1,
        "image": "male.png",
        "notes": "test",
        "creator_id": null,
        "email_verified_at": "2022-09-28 10:45:20",
        "order_error": 1,
        "item_error": 1
    }
}
```