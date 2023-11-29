# Retrieve items with query builder

`endpoint: api/v1/items`

`Method: GET`

**searchable query fields**

| Name            | Type                                          |
|-----------------|-----------------------------------------------|
| client_id       | integer/array                                 |
| sku             | string  or separated by comma or array        |
| first_name      | string                                        |
| last_name       | string                                        |
| telephone       | string                                        |
| email           | string                                        |
| company         | string                                        |
| order_from      | date                                          |
| order_to        | Date                                          |
| arrival_from    | Date                                          |
| arrival_to      | Date                                          |
| postal_code     | string                                        |
| country_id      | integer                                       |
| province_id     | integer                                       | 
| order_status_id | integer or separated by comma or array        |
| status          | boolean                                       |
| ready           | boolean                                       |
| processing_type | number                                        |
| sort_by         | any of above field                            |
| sort_order      | DESC/ASC                                      |
| limit           | number(<200)                                  |
| list            | count/take/auto-complete (default: paginated) |

* maximum of limit < 200 per page.
* list is keyword , its value could be in "count, take, auto-complete".
* paginated data will give out if no flag of list.

# response

```json

```