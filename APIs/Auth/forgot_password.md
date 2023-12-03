# Forgot password

### URL
```text
api/v1/password/forgot-password`
```
### Method
```text
POST
```


### Parameters

| Name  | Type  | Required | Default | Description |
|-------|-------|----------|---------|-------------|
| email | email | Y        |         |             |

### Auth required 
```text
NO
```
### Header
```text
Content-Type: application/json
Accept: application/json
```


### Request example
```json
{
  "email": "your-email@domain.com"
}
```
### Success response

```json
{
    "success": false,
    "message": "Email could not be sent to this email address",
    "data": []
}
```