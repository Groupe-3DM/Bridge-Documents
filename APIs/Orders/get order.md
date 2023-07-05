# Bridge-Documents

**searchable fields**

> Method: GET

> endpoint: api/v1/orders

> example: api/v1/orders?client_id=1234&order_number=abc_123&........


| Name             | Type                                          |
|------------------|-----------------------------------------------|
| id | number/array                                  | 
| order_number| string                                        |
| client_id| number/array                                  |
| sku | string                                        |
| first_name | string                                        |
| last_name | string                                        |
| telephone | string                                        |
| email | string                                        |
| company | string                                        |
| order_from | date                                          |
| order_to | Date                                          |
| arrival_from | Date                                          |
| arrival_to | Date                                          |
| postal_code | string                                        |
| country_id | number                                        |
| province_id | number                                        | 
| order_status_id| number                                        |
| order_type_id| number/array                                  |
| ready | boolean                                       |
| processing_type | number                                        |
| sort_by | any of above field                            |
| sort_order | DESC/ASC                                      |
|limit| number(<200)                                  |
|list| count/take/auto-complete (default: paginated) |

# response

```json
{
    "success": true,
    "message": "Operation has been successfully completed!",
    "data": {
        "current_page": 1,
        "data": [
         ...
        ],
        "first_page_url": ".../api/v1/orders?page=1",
        "from": 1,
        "last_page": 4,
        "last_page_url": ".../api/v1/orders?page=4",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "http://lara3dmapi.test/api/v1/orders?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": "http://lara3dmapi.test/api/v1/orders?page=2",
                "label": "2",
                "active": false
            },
            {
                "url": "http://lara3dmapi.test/api/v1/orders?page=3",
                "label": "3",
                "active": false
            },
            {
                "url": "http://lara3dmapi.test/api/v1/orders?page=4",
                "label": "4",
                "active": false
            },
            {
                "url": "http://lara3dmapi.test/api/v1/orders?page=2",
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": ".../api/v1/orders?page=2",
        "path": ".../api/v1/orders",
        "per_page": 15,
        "prev_page_url": null,
        "to": 15,
        "total": 48
    }
}
```