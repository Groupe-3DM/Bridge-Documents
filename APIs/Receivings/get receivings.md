# Retrieve a list of all purchase orders.



`Method: GET`

`endpoint: api/v1/items`

**searchable query fields**

| Name             | Type                                          |
|------------------|-----------------------------------------------|
| client_id| number/array                                  |
| sku | string                                        |
| sort_by | any of above field                            |
| sort_order | DESC/ASC                                      |
|limit| number(<200)                                  |
|list| count/take/auto-complete (default: paginated) |

# response

```json
```