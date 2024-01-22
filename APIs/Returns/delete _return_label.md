# Retrieve return labels

### URL

```text
api/v1/admin/return-labelS/:id
```

### Method

```text
DELETE
```

### Parameters

| Name            | Type    | Required | Default | Description                                  |
|-----------------|---------|----------|---------|----------------------------------------------|
| tracking_number | string  |          |         |                                              |
| order_id        | integer |          |         |                                              |
| carrier_id      | integer |          |         |                                              |
| sort_order      | string  |          |         | DESC/ASC                                     |
| limit           | integer |          | 15      | max<200                                      |
| list            | string  |          |         | all/count/take/auto-complete                 |

### Note

```text


* paginated data will give out if no flag of list
```

### Auth required (Admin)

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

```