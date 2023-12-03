# Auth: password reset

### URL
```text
api/v1/password/reset
```

### Method
```text
POST
```

### Parameters

| Name                  | Type   | Required | Default | Description             |
|-----------------------|--------|----------|---------|-------------------------|
| email                 | email  | Y        |         |                         |
| token                 | string | Y        |         | token in the email link |
| password              | string | Y        |         |                         |
| password-confirmation | string | Y        |         |                         |

### Auth required
```text
NO
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
    "success": false,
    "message": "Email could not be sent to this email address",
    "data": []
}
```



