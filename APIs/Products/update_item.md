# Update an item

### URL

```text
api/v1/items/:id
```

### Method

```text
PUT
```

### Parameters

| Name                             | Type    | Required                  | Default | Description                             |
|----------------------------------|---------|---------------------------|---------|-----------------------------------------|
| client_id                        | id      |                           |         |                                         |
| sku                              | string  |                           |         |                                         |
| item_type_id                     | id      |                           |         | [APIs](../Others/get_item_types.md)     |
| supply_type_id                   | id      | Y if item_type_id=4       |         | [APIs](../Others/get_supply_types.md)   |
| order_unit                       | integer |                           |         | >0                                      |
| length_class_id                  | id      |                           |         | [APIs](../Others/get_length_classes.md) |
| weight_class_id                  | id      |                           |         | [APIs](../Others/get_weight_classes.md) |
| barcoded                         | boolean |                           |         | 1 yes, 0 no                             |
| manufacturer_code                | string  |                           |         |                                         |
| upc                              | string  |                           |         |                                         |
| group                            | string  |                           |         |                                         |
| family                           | string  |                           |         |                                         |
| color                            | string  |                           |         |                                         |
| size                             | string  |                           |         |                                         |
| material                         | string  |                           |         |                                         |
| category                         | string  |                           |         |                                         |
| sub_category                     | string  |                           |         |                                         |
| department                       | string  |                           |         |                                         |
| sub_department                   | string  |                           |         |                                         |
| supplier_code                    | string  |                           |         |                                         |
| item_linguistic_id               | id      |                           |         | [APIs](../Others/get_linguistics.md)    |
| season                           | string  |                           |         |                                         |
| year                             | integer |                           |         |                                         |
| quarantine_days                  | boolean |                           |         |                                         |
| pre_alert_days                   | integer |                           |         | >=0                                     |
| low_level_warning                | integer |                           |         | >=0                                     |
| hazmat                           | boolean |                           |         | 1 yes, 0 no                             |
| currency_id                      | id      |                           |         | [APIs](../Others/get_currencies.md)     |
| cost                             | decimal |                           |         | >=0                                     |
| kit_surcharge                    | boolean |                           |         | 1 yes, 0 no                             |
| ambient                          | boolean |                           |         | 1 yes, 0 no                             |
| cold_chain                       | boolean |                           |         | 1 yes, 0 no                             |
| controlled                       | boolean |                           |         | 1 yes, 0 no                             |
| restricted_access                | boolean |                           |         | 1 yes, 0 no                             |
| restricted_ecomm                 | boolean |                           |         | 1 yes, 0 no                             |
| restricted_precursor             | boolean |                           |         | 1 yes, 0 no                             |
| lot_expiry_needed                | boolean |                           |         | 1 yes, 0 no                             |
| serial_number                    | boolean |                           |         | 1 yes, 0 no                             |
| air_ground_control               | boolean |                           |         | 1 yes, 0 no                             |
| measurements                     | array   |                           |         |                                         |
| measurements.*                   | array   | Y if measurements present |         |                                         |
| measurements.*.quantity          | integer | Y                         |         | >0                                      |
| measurements.*.uom_type_id       | integer | Y                         |         | [APIs](../Others/get_uom_types.md)      |
| measurements.*.length            | decimal | Y                         |         | >0                                      |
| measurements.*.weight            | decimal | Y                         |         | >0                                      |
| measurements.*.width             | decimal | Y                         |         | >0                                      |
| measurements.*.height            | decimal | Y                         |         | >0                                      |
| measurements.*.barcode           | string  | Y                         |         |                                         |
| measurements.*.description       | string  | Y                         |         |                                         |
| descriptions                     | array   | Y                         |         | (size=2, en and fr)                     |
| descriptions.*                   | array   | Y                         |         |                                         |
| descriptions.*.description       | string  | Y                         |         |                                         |
| descriptions.*.language_id       | id      | Y                         |         | [APIs](../Others/get_languages.md)      |
| kits                             | array   | Y if item_type_id=2       |         |                                         |
| kits.*                           | array   | Y                         |         |                                         |
| kits.*.quantity                  | integer | Y                         |         | >0                                      |
| kits.*.child_item_id             | id      | Y                         |         |                                         |
| kits.*.mix_lot                   | boolean | Y                         |         | 1 yes, 0 no                             |
| kits.*.lot_kit                   | boolean | Y                         |         | 1 yes, 0 no                             |
| kits.*.populate_order            | boolean | Y                         |         |                                         |
| hazmats                          | array   | Y if hazmat               |         |                                         |
| hazmats.un_number                | string  | Y                         |         |                                         |
| hazmats.class                    | string  | Y                         |         |                                         |
| hazmats.packing_group            | string  | Y                         |         |                                         |
| hazmats.quantity                 | integer | Y                         |         | >0                                      |
| hazmats.description              | string  | Y                         |         |                                         |
| manufacturer                     | array   |                           |         |                                         |
| manufacturer.country_id          | id      |                           |         | [APIs](../Others/get_countries.md)      |
| manufacturer.original_country_id | id      |                           |         | [APIs](../Others/get_countries.md)      |
| manufacturer.province_id         | id      |                           |         | [APIs](../Others/get_provinces.md)      |
| manufacturer.name                | string  |                           |         |                                         |
| manufacturer.postal_code         | string  |                           |         |                                         |
| manufacturer.code                | string  |                           |         |                                         |
| manufacturer.mid                 | string  |                           |         |                                         |
| manufacturer.phone               | string  |                           |         |                                         |
| manufacturer.city                | string  |                           |         |                                         |
| manufacturer.address1            | string  |                           |         |                                         |
| manufacturer.address2            | string  |                           |         |                                         |
| manufacturer.description         | string  |                           |         |                                         |
| manufacturer.sale_price          | decimal |                           |         | >=0                                     |
| manufacturer.international_ship  | boolean |                           |         | 1 yes, 0 no                             |

### Note

```text

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
{
  "descriptions": [
    {
      "language_id": 1,
      "description": "English description"
    },
    {
      "language_id": 2,
      "description": "French description"
    }
  ],
  "measurements": [
    {
      "quantity": 1,
      "length": 1,
      "width": 1,
      "height": 1,
      "barcode": "abcd4567",
      "description": "test",
      "uom_type_id": 1,
      "weight": 1
    }
  ]
}
```

### Success response

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "client_id": 1,
    "sku": "abcd4567",
    "item_type_id": 1,
    "supply_type_id": null,
    "item_status_id": 1,
    "order_unit": 1,
    "barcoded": true,
    "manufacturer_code": null,
    "upc": null,
    "group": null,
    "family": null,
    "color": null,
    "size": null,
    "material": null,
    "category": null,
    "sub_category": null,
    "department": null,
    "sub_department": null,
    "supplier_code": null,
    "item_linguistic_id": null,
    "season": null,
    "year": null,
    "supplier_id": null,
    "quarantine_days": 0,
    "pre_alert_days": 0,
    "low_level_warning": 0,
    "currency_id": null,
    "cost": 0,
    "kit_surcharge": 0,
    "length_class_id": 1,
    "weight_class_id": 1,
    "image": null,
    "ambient": false,
    "cold_chain": false,
    "controlled": false,
    "hazmat": null,
    "restricted_access": false,
    "restricted_pharma": false,
    "restricted_ecomm": false,
    "restricted_precursor": false,
    "lot_expiry_needed": false,
    "serial_number": 0,
    "base_uom_type_id": 1,
    "client_name": "GROUPE 3-DM",
    "id": 459522,
    "available": 0,
    "unavailable": 0,
    "on_hand": 0,
    "committed": 0,
    "kits": [],
    "descriptions": [
      {
        "item_id": 459522,
        "language_id": 1,
        "description": "English description"
      },
      {
        "item_id": 459522,
        "language_id": 2,
        "description": "French description"
      }
    ],
    "manufacturer": null,
    "measurements": [
      {
        "item_id": 459522,
        "uom_type_id": 1,
        "uom_hierarchy": 1,
        "quantity": 1,
        "weight": "1.0000",
        "length": "1.0000",
        "height": "1.0000",
        "width": "1.0000",
        "barcode": "abcd4567",
        "description": "test",
        "id": 429040
      }
    ]
  }
}
```

