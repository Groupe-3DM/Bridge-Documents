# Create an item

`endpoint: api/v1/items`

`Method: POST`

### Parameters

| Name                                | Type    | Mandatory     |
|-------------------------------------|---------|---------------|
| client_id                           | integer | Y             |
| sku                                 | string  |               |
| item_type_id                        | integer | Y             |
| supply_type_id                      | integer | Y             |
| item_status_id                      | integer |               |
| order_unit                          | integer |               |
| length_class_id                     | integer |               |
| weight_class_id                     | integer | Y             |
| barcoded                            | boolean |               |
| manufacturer_code                   | string  | Y             |
| upc                                 | string  | Y             |
| group                               | string  | Y             |
| family                              | string  |               |
| color                               | string  |               |
| size                                | string  |               |
| material                            | string  | Y             |
| category                            | string  |               |
| sub_category                        | string  |               |
| department                          | string  |               |
| sub_department                      | string  |               |
| supplier_code                       | string  |               |
| item_linguistic_id                  | integer |               |
| season                              | string  |               |
| year                                | integer |               |
| supplier_id                         | integer |               |
| quarantine_days                     | boolean |               |
| pre_alert_days                      | integer |               |
| low_level_warning                   | integer |               |
| hazmat                              | boolean |               |
| currency_id                         | string  |               |
| cost                                | decimal |               |
| kit_surcharge                       | boolean |               |
| ambient                             | boolean |               |
| cold_chain                          | boolean |               |
| controlled                          | boolean |               |
| restricted_access                   | boolean |               |
| restricted_ecomm                    | boolean |               |
| restricted_precursor                | boolean |               |
| lot_expiry_needed                   | boolean |               |
| serial_number                       | boolean |               |
| air_ground_control                  | boolean |               |
| measurements                        | array   | Y             |
| measurements.*                      | array   | Y             |
| measurements.*.quantity             | integer | Y             |
| measurements.*.uom_type_id          | integer | Y             |
| measurements.*.length               | decimal | Y             |
| measurements.*.weight               | decimal | Y             |
| measurements.*.width                | decimal | Y             |
| measurements.*.height               | decimal | Y             |
| measurements.*.barcode              | boolean | Y             |
| measurements.*.description          | string  | Y             |
| descriptions                        | array   | Y (size=2)    |
| descriptions.*                      | array   | Y             |
| descriptions.*.description          | string  | Y             |
| descriptions.*.language_id          | integer | Y             |
| kits                                | array   |               |
| kits.*                              | array   | Y             |
| kits.*.quantity                     | integer | Y             |
| kits.*.child_item_id                | integer | Y             |
| kits.*.mix_lot                      | boolean | Y             |
| kits.*.lot_kit                      | boolean | Y             |
| kits.*.populate_order               | boolean | Y             |
| hazmats                             | array   | Y (if hazmat) |
| hazmats.*                           | array   | Y             |
| hazmats.*.un_number                 | string  | Y             |
| hazmats.*.class                     | string  | Y             |
| hazmats.*.packing_group             | string  | Y             |
| hazmats.*.quantity                  | integer | Y             |
| hazmats.*.description               | string  | Y             |
| manufacturers                       | array   |               |
| manufacturers.*                     | array   | Y             |
| manufacturers.*.country_id          | integer | Y             |
| manufacturers.*.original_country_id | integer | Y             |
| manufacturers.*.province_id         | integer | Y             |
| manufacturers.*.name                | string  | Y             |
| manufacturers.*.postal_code         | string  | Y             |
| manufacturers.*.code                | string  | Y             |
| manufacturers.*.mid                 | string  | Y             |
| manufacturers.*.phone               | string  | Y             |
| manufacturers.*.city                | string  | Y             |
| manufacturers.*.address1            | string  | Y             |
| manufacturers.*.address2            | string  | Y             |
| manufacturers.*.description         | string  | Y             |
| manufacturers.*.sale_price          | decimal | Y             |
| manufacturers.*.international_ship  | boolean | Y             |

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