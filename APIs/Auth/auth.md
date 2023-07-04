# Auth

**Data constraints(api/v1/login)**
```json
{
  "email": "[required|string|email]",
  "password": "[required|string]"
}
```
**Data constraints(api/v1/password/forgot-password)**

```json
{
  "email": "[required|string]"
}
```
**Data constraints(api/v1/password/reset)**

```json
{
  "email": "[required|string]",
  "token": "[required|string]",
  "password-confirmation": "[required|string]",
  "password": "[required|string]"


}
```

**Data constraints(api/v1/me)**
```json
{
  "Authorization": "required|format: Bearer {token}"
}
```


**URL** 

api/v1/login(POST)

api/v1/me (GET)

api/v1/password/reset(POST)

api/v1/password/forgot-password(POST)
