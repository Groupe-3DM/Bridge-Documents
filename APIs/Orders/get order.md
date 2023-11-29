# Get a list of orders with query builder

`endpoint: api/v1/orders`

`Method: GET`


**searchable query fields**

| Name            | Type                                          |
|-----------------|-----------------------------------------------|
| order_number    | string                                        |
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
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "id": 242,
    "client_id": 9999,
    "order_number": "1041",
    "internal_order": "9999-01",
    "order_date": "2023-03-22 11:47:53",
    "status": 1,
    "order_status_id": 17,
    "order_type_id": null,
    "processing_type_id": null,
    "parent_id": null,
    "first_name": "test",
    "last_name": "etst",
    "email": "",
    "company": "",
    "telephone": "",
    "address1": "328 Rue Avro",
    "address2": "",
    "address3": null,
    "postal_code": "H9R 5W5",
    "apt_num1": null,
    "apt_num2": null,
    "city": "Pointe-Claire",
    "province_id": 612,
    "country_id": 38,
    "reference1": null,
    "reference2": null,
    "packing_slip_note": null,
    "pick_up": 0,
    "inside_delivery": 0,
    "lift_gate_required": 0,
    "ready": 1,
    "is_master": 0,
    "quantity_ordered": 0,
    "quantity_in_process": 0,
    "quantity_shipped": 0,
    "quantity_backorder": 0,
    "batch_id": null,
    "process_date": null,
    "deliver_by_date": null,
    "handling_priority": 0,
    "processing_priority": 0,
    "temperature_control": null,
    "hazmat": 0,
    "appointment_required": 0,
    "order_handling": 0,
    "signature_required": 0,
    "ambient_control": 0,
    "air_ground_control": 0,
    "handling_instruction": null,
    "dangerous_goods": 0,
    "language_id": null,
    "carrier_id": null,
    "service_id": null,
    "packing_slips": null,
    "note": null,
    "custom_reference_no": null,
    "label_provided": 0,
    "shipping_label_file": null,
    "client_po": null,
    "carrier_service": null,
    "picking_method_id": null,
    "client_order_id": "5105233264835",
    "carrier": null,
    "trackings": null,
   
    "client_name": "TEST",
    "order_items": [
      {
        "id": 427,
        "order_id": 242,
        "item_id": 4273,
        "descriptions": "New test sku 1",
        "quantity_ordered": 1,
        "sku": "NewTestSku1",
        "lot": "",
        "expiry_date": null,
        "unit_value": "0.0000",
        "order_item_status_id": 1,
        "uom_type_id": 1,
        "created_by": null,
        "created_at": "2023-05-11T15:00:53.000000Z",
        "sale_price": "0.00"
      },
      {
        "id": 428,
        "order_id": 242,
        "item_id": 4274,
        "descriptions": "New test sku 2",
        "quantity_ordered": 1,
        "sku": "NewTestSku2",
        "lot": "",
        "expiry_date": null,
        "unit_value": "0.0000",
        "order_item_status_id": 1,
        "uom_type_id": 1,
        "created_by": null,
        "created_at": "2023-05-11T15:00:53.000000Z",
        "sale_price": "0.00"
      }
    ]
  }
}
```