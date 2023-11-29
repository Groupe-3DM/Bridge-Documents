# Create an item

`endpoint: api/v1/items`

`Method: POST`

### Parameters

| Name                               | Type    | Mandatory |
|------------------------------------|---------|-----------|
| client_id                          | integer | Y         |
| sku                                | string  |           |
| item_type_id                       | string  | Y         |
| supply_type_id                     | string  | Y         |
| item_status_id                     | string  |           |
| order_unit                         | string  |           |
| length_class_id                    | string  |           |
| weight_class_id                    | string  | Y         |
| barcoded                           | string  |           |
| manufacturer_code                  | string  | Y         |
| upc                                | string  | Y         |
| group                              | string  | Y         |
| family                             | string  |           |
| color                              | string  |           |
| size                               | string  |           |
| material                           | string  | Y         |
| category                           | string  |           |
| sub_category                       | string  |           |
| department                         | string  |           |
| sub_department                     | boolean |           |
| supplier_code                      | boolean |           |
| item_linguistic_id                 | boolean |           |
| season                             | boolean |           |
| year                               | boolean |           |
| supplier_id                        | boolean |           |
| quarantine_days                    | boolean |           |
| pre_alert_days                     | integer |           |
| low_level_warning                  | integer |           |
| hazmat                             | string  |           |
| currency_id                        | string  |           |
| cost                               | date    |           |
| kit_surcharge                      | boolean |           |
| ambient                            | boolean |           |
| cold_chain                         | boolean |           |
| controlled                         | boolean |           |
| restricted_access                  | boolean |           |
| restricted_ecomm                   | boolean |           |
| restricted_precursor               | boolean |           |
| lot_expiry_needed                  | boolean |           |
| serial_number                      | boolean |           |
| air_ground_control                 | boolean |           |
| measurements                       | array   | Y         |
| measurements.*                     | array   | Y         |
| measurements.*.quantity            | integer | Y         |
| measurements.*.uom_type_id         | integer | Y         |
| measurements.*.length              | integer | Y         |
| measurements.*.weight              | integer | Y         |
| measurements.*.width               | integer | Y         |
| measurements.*.height              | integer | Y         |
| measurements.*.barcode             | date    | Y         |
| measurements.*.description         | integer | Y         |
| descriptions                       | array   | Y         |
| descriptions.*                     | array   | Y         |
| descriptions.*.description         | integer | Y         |
| descriptions.*.language_id         | integer | Y         |
| kits                               | array   |           |
| kits.*                             | array   | Y         |
| kits.*.quantity                    | integer | Y         |
| kits.*.child_item_id               | integer | Y         |
| kits.*.mix_lot                     | integer | Y         |
| kits.*.lot_kit                     | integer | Y         |
| kits.*.populate_order              | integer | Y         |
| hazmats                            | array   |           |
| hazmats.*                          | array   | Y         |
| hazmats.*.un_number                | integer | Y         |
| hazmats.*.class                    | integer | Y         |
| hazmats.*.packing_group            | integer | Y         |
| hazmats.*.quantity                 | integer | Y         |
| hazmats.*.description              | integer | Y         |
| manufacturers                      | array   |           |
| manufacturers.*                    | array   | Y         |
| manufacturers.*.country_id         | integer | Y         |
| manufacturers.*.province_id        | integer | Y         |
| manufacturers.*.name               | integer | Y         |
| manufacturers.*.postal_code        | integer | Y         |
| manufacturers.*.code               | integer | Y         |
| manufacturers.*.mid                | integer | Y         |
| manufacturers.*.phone              | integer | Y         |
| manufacturers.*.city               | integer | Y         |
| manufacturers.*.address1           | integer | Y         |
| manufacturers.*.address2           | integer | Y         |
| manufacturers.*.description        | integer | Y         |
| manufacturers.*.sale_price         | integer | Y         |
| manufacturers.*.international_ship | integer | Y         |

# Response:

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "client_id": 1,
    "order_number": 1689625979,
    "order_date": "2023-09-09 11:11:11",
    "email": null,
    "first_name": "jon",
    "last_name": null,
    "address1": "222 ave mntril",
    "province_id": 121,
    "country_id": 38,
    "city": "kkkkkkk",
    "telephone": null,
    "company": null,
    "postal_code": "kkkk",
    "address2": null,
    "address3": null,
    "apt_num1": null,
    "apt_num2": null,
    "reference1": null,
    "reference2": null,
    "parent_id": null,
    "packing_slip_note": null,
    "handling_priority": 0,
    "processing_priority": false,
    "is_master": false,
    "ready": 0,
    "order_type_id": 1,
    "order_status_id": 15,
    "pick_up": false,
    "inside_delivery": false,
    "lift_gate_required": false,
    "hazmat": false,
    "order_handling": false,
    "appointment_required": false,
    "temperature_control": false,
    "dangerous_goods": false,
    "language_id": 1,
    "warehouse_id": 12,
    "carrier_id": null,
    "transaction": null,
    "carrier_service": null,
    "service_id": null,
    "note": null,
    "custom_reference_no": null,
    "created_by": "Genming Zhao",
    "updated_by": "Genming Zhao",
    "deliver_by_date": null,
    "signature_required": false,
    "ambient_control": false,
    "air_ground_control": 0,
    "ship_onpty3": false,
    "pty3_account": null,
    "label_provided": false,
    "tracking_number": null,
    "client_po": null,
    "status": 1,
    "picking_method_id": 1,
    "processing_type_id": 2,
    "internal_order": "1-18",
    "updated_at": "2023-07-17T20:32:59.000000Z",
    "created_at": "2023-07-17T20:32:59.000000Z",
    "id": 341,
    "warehouse_name": "3DM - AVRO",
    "client_name": "Group 3-DM",
    "order_items": [
      {
        "id": 583,
        "order_id": 341,
        "item_id": 1,
        "descriptions": "",
        "quantity_ordered": 1,
        "sku": "sku1236",
        "lot": "",
        "expiry_date": null,
        "unit_value": "0.0000",
        "order_item_status_id": 1,
        "uom_type_id": 1,
        "created_by": "Genming Zhao",
        "created_at": "2023-07-17T20:32:59.000000Z",
        "sale_price": "3.00"
      }
    ]
  }
}
```