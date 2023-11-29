# Update an item

 

 `endpoint: api/v1/items/{id}`

  `Method: PUT`

# Response

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

