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
    "id": 4604,
    "client_id": 1,
    "sku": "232R-90-0-100",
    "upc": null,
    "manufacturer_code": null,
    "kit_surcharge": "0.0000",
    "item_type_id": 1,
    "supply_type_id": null,
    "order_unit": 9,
    "quarantine_days": 0,
    "pre_alert_days": 0,
    "low_level_warning": 0,
    "department": null,
    "sub_department": null,
    "category": null,
    "sub_category": null,
    "item_linguistic_id": null,
    "length_class_id": 1,
    "weight_class_id": 1,
    "season": null,
    "year": null,
    "supplier_code": null,
    "family": null,
    "group": null,
    "material": null,
    "color": null,
    "size": null,
    "image": null,
    "cost": "0.0000",
    "currency_id": null,
    "item_status_id": 1,
    "ambient": 0,
    "cold_chain": 0,
    "restricted_access": 0,
    "controlled": 0,
    "hazmat": 0,
    "restricted_pharma": 0,
    "restricted_ecomm": 0,
    "restricted_precursor": 0,
    "lot_expiry_needed": 0,
    "supplier_id": null,
    "barcoded": 1,
    "serial_number": 0,
    "item_category_id": null,
    "client_name": "Group 3-DM",
    "available": 0,
    "unavailable": 0,
    "descriptions": [
      {
        "id": 640,
        "item_id": 4604,
        "language_id": 1,
        "description": "1"
      },
      {
        "id": 641,
        "item_id": 4604,
        "language_id": 2,
        "description": "2"
      }
    ],
    "measurements": [
      {
        "id": 328,
        "item_id": 4604,
        "uom_type_id": 1,
        "quantity": 1,
        "weight": "1.0000",
        "length": "1.0000",
        "height": "1.0000",
        "width": "1.0000",
        "barcode": "899",
        "description": "test"
      },
      {
        "id": 329,
        "item_id": 4604,
        "uom_type_id": 2,
        "quantity": 8,
        "weight": "1.0000",
        "length": "1.0000",
        "height": "1.0000",
        "width": "1.0000",
        "barcode": "8990",
        "description": "8 units in one box"
      }
    ],
    "manufacturer": null,
    "kits": [],
    "hazmats": null
  }
}
```