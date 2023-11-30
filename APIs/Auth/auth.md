# Auth

`endpoint: api/v1/login`

`method: POST`

### Parameters

| Name     | Type   | Mandatory |
|----------|--------|-----------|
| email    | email  | Y         |
| password | string | Y         |
--------------------------------------------------------
`endpoint: api/v1/password/forgot-password`

`method: POST`

### Parameters

| Name     | Type   | Mandatory |
|----------|--------|-----------|
| email    | email  | Y         |

------------------------------------------------------
`endpoint: api/v1/password/reset`

`method: POST`

### Parameters

| Name                  | Type   | Mandatory  |
|-----------------------|--------|------------|
| email                 | email  | Y          |
| token                 | string | Y          |
| password              | string | Y          |
| password-confirmation | string | Y          |


------------------------------------------------

`endpoint: api/v1/me`

`method: GET`



