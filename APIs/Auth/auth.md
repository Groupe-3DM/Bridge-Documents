# Auth

`endpoint: api/v1/login`
### Method: `POST`
### parameters:
| Name     | Type   | mandatory |
|----------|--------|---------|
| email    | email  | Y       |
| password | string | Y       |
```json

```
`endpoint: api/v1/password/forgot-password`

### Method: `POST`
### parameters:
| Name     | Type   | mandatory |
|----------|--------|---------|
| email    | email  | Y       |

```json

```
`endpoint: api/v1/password/reset`

### Method: `POST`
### parameters:
| Name                  | Type   | mandatory |
|-----------------------|--------|---------|
| email                 | email  | Y       |
| token                 | string | Y       |
| password              | string | Y       |
| password-confirmation | string | Y       |
```json
{
  
}
```

`endpoint: api/v1/me`

### Method: `GET`



