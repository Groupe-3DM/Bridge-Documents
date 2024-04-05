# Retrieve a list of order statuses with query builder

### URL

```text
api/v1/order-statuses
```

### Method

```text
GET
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

| item_type_id | name                |
|--------------|---------------------|
| 1            | Received            |
| 2            | Released            |
| 3            | Batched             |
| 4            | Picking in progress |
| 5            | Awaiting Packing    |
| 6            | Packing in progress |
| 7            | Partial             |
| 8            | Packed              |
| 9            | Awaiting pick-up    |
| 10           | Partial shipped     |
| 11           | Shipped             |
| 12           | Backorder           |
| 13           | On-Hold             |
| 14           | Cancelled           |
| 15           | Receiving           |
| 16           | Awaiting shipping   |
| 17           | Error               |
