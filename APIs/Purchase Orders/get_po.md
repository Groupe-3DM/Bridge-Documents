# Retrieve a list of purchase orders with query builder

### URL

```text
api/v1/items/:id
```

### Method

```text
GET
```

### Parameters

| Name                        | Type    | Required | Default | Description                                        |
|-----------------------------|---------|----------|---------|----------------------------------------------------|
| client_id                   | id      |          |         |                                                    |
| supplier_id                 | id      |          |         |                                                    |
| po_number                   | string  |          |         |                                                    |
| purchase_order_condition_id | id      |          |         | [APIs](../Others/get_purchase_order_conditions.md) |
| purchase_order_status_id    | id      |          |         | [APIs](../Others/get_purchase_order_statuses.md)   |
| warehouse_id                | id      |          |         | [APIs](../Others/get_warehouses.md)                |
| sort_by                     | string  |          |         | any of above field                                 |
| sort_order                  | string  |          |         | DESC/ASC                                           |
| limit                       | integer |          | 15      | (<200)                                             |
| list                        | string  |          |         | all/count/take/auto-complete (default: paginated)  |



### Note

```text
query's example: client_id=1&po_number=xxxx&limit=20&list=all
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

### Request example

```json

```

### Success response

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "data": [
      {
        "id": 3,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": null,
        "warehouse_name": null,
        "po_number": null,
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 0,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 6,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": null,
        "warehouse_name": null,
        "po_number": "1-po-1693574938",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 7,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": null,
        "warehouse_name": null,
        "po_number": "1-po-1693575574",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 8,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": null,
        "warehouse_name": null,
        "po_number": "1-po-1693575693",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 9,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": null,
        "warehouse_name": null,
        "po_number": "1-po-1693575740",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 10,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": null,
        "warehouse_name": null,
        "po_number": "1-po-1693575903",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 11,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": null,
        "warehouse_name": null,
        "po_number": "1-po-1693576027",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 12,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": null,
        "warehouse_name": null,
        "po_number": "1-po-1693576173",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 1000,
        "quantity_received": 0,
        "purchase_order_condition_id": 3,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 13,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": 12,
        "warehouse_name": null,
        "po_number": "1-po-1695649841",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 14,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": 12,
        "warehouse_name": null,
        "po_number": "1-po-1695649992",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 15,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": 12,
        "warehouse_name": null,
        "po_number": "1-po-1695650101",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 16,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": 12,
        "warehouse_name": null,
        "po_number": "1-po-1695650538",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 17,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": 12,
        "warehouse_name": null,
        "po_number": "1-po-1695650653",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 18,
        "client_id": 1,
        "client_name": null,
        "warehouse_id": 12,
        "warehouse_name": null,
        "po_number": "1-po-1695650764",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      },
      {
        "id": 24,
        "client_id": 1,
        "client_name": "Group 3-DM",
        "warehouse_id": 12,
        "warehouse_name": "3DM - AVRO",
        "po_number": "1-po-1697226710",
        "supplier_id": null,
        "supplier_name": null,
        "quantity_expected": 100,
        "quantity_received": 0,
        "purchase_order_condition_id": 1,
        "purchase_order_status_id": 1,
        "shipping_method_id": 1,
        "date_expected": "2021-09-01",
        "date_received": null,
        "time_allotted_start": null,
        "time_allotted_end": null,
        "quantity_in_progress": 0
      }
    ],
    "current_page": 1,
    "last_page": 3,
    "from": 1,
    "to": 15,
    "total": 35,
    "per_page": 15
  }
}
```