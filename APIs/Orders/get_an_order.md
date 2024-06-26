# Retrieve an order

### URL

```text
api/v1/orders/:id
```

### Method

```text
GET
```

### Parameters


| Name                           | Type    | Required | Default | Description |
|--------------------------------|---------|----------|---------|-------------|

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

```

### Success response


```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "id": 326,
    "client_id": 9999,
    "order_number": "1112",
    "order_date": "2023-05-31 11:31:38",
    "order_state_id": 1,
    "order_status_id": 14,
    "order_type_id": null,
    "processing_type_id": null,
    "parent_id": null,
    "first_name": "3DM",
    "last_name": "Ship",
    "email": "xxxxxxxxxxxxxxm",
    "company": "3DM",
    "telephone": "+15146959922",
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
    "warehouse_id": null,
    "carrier_id": null,
    "service_id": null,
    "packing_slips": null,
    "note": null,
    "custom_reference_no": null,
    "label_provided": 0,
    "shipping_label_file": null,
    "tracking_number": null,
    "picking_method_id": null,
    "client_order_id": "5181111435459",
    "carrier": null,
    "trackings": null,
    "client_name": "TEST",
    "order_items": [
      {
        "id": 551,
        "order_id": 326,
        "item_id": 4377,
        "descriptions": "Fun test productModifyTitleTestadd",
        "quantity_ordered": 1,
        "sku": "YESTESTSKU",
        "lot": "",
        "expiry_date": null,
        "unit_value": "0.0000",
        "order_item_status_id": 1,
        "uom_type_id": 1,
        "created_by": null,
        "created_at": "2023-06-03T01:28:01.000000Z",
        "sale_price": "0.00"
      },
      {
        "id": 552,
        "order_id": 326,
        "item_id": 4374,
        "descriptions": "FINAL TEST1",
        "quantity_ordered": 1,
        "sku": "FT1",
        "lot": "",
        "expiry_date": null,
        "unit_value": "0.0000",
        "order_item_status_id": 1,
        "uom_type_id": 1,
        "created_by": null,
        "created_at": "2023-06-03T01:28:01.000000Z",
        "sale_price": "0.00"
      }
    ]
  }
}
```