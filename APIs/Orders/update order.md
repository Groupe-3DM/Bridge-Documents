# Update an order

 `method: PUT`

 `endpoint: api/v1/orders/{id}`


` * order status id and order state can not be updated.`

### data body
```json
{
  "order_date"               : "sometimes|date_format:Y-m-d H:i:s",
  "first_name"               : "sometimes|string|max:".Constant::MAX_STRING_LENGTH,
  "address1"                 : "sometimes|string|max:".Constant::MAX_STRING_LENGTH,
  "postal_code"              : "sometimes|string|max:".Constant::MAX_STRING_LENGTH,
  "city"                     : "sometimes|string|max:".Constant::MAX_STRING_LENGTH,
  "province_id"              : "sometimes|exists:provinces,id",
  "country_id"               : "sometimes|exists:countries,id",
  "telephone"                : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "last_name"                : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "company"                  : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "email"                    : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "reference1"               : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "reference2"               : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "packing_slip_note"        : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "items"                    : "nullable|array",
  "items.*"                  : "nullable|array",
  "apt_num1"                 : "sometimes|string|nullable|max:".Constant::MAX_STRING_LENGTH,
  "apt_num2"                 : "sometimes|string|nullable|max:".Constant::MAX_STRING_LENGTH,
  "address2"                 : "sometimes|string|nullable|max:".Constant::MAX_STRING_LENGTH,
  "pick_up"                  : "sometimes|nullable|boolean",
  "inside_delivery"          : "sometimes|nullable|boolean",
  "lift_gate_required"       : "sometimes|nullable|boolean",
  "handling_priority"        : "sometimes|nullable|boolean",
  "temperature_control"      : "sometimes|nullable|in:0,1,2",
  "hazmat"                   : "sometimes|nullable|boolean",
  "appointment_required"     : "sometimes|nullable|boolean",
  "order_handling"           : "sometimes|nullable|boolean",
  "handling_instruction"     : "sometimes|nullable|string|max:".Constant::MAX_TEXT_LENGTH,
  "dangerous_goods"          : "sometimes|nullable|boolean",
  "language_id"              : "sometimes|nullable|exists:languages,id",
  "transaction"              : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "carrier_id"               : "sometimes|nullable|exists:carriers,id",
  "carrier_service"          : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "service_id"               : "sometimes|nullable|exists:services,id",
  "note"                     : "sometimes|nullable|string|max:".Constant::MAX_TEXT_LENGTH,
  "custom_reference_no"      : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  " deliver_by_date"         : "sometimes|nullable|date_format:Y-m-d",
  "signature_required"       : 'sometimes|nullable|boolean',
  "ambient_control"          : 'sometimes|nullable|boolean',
  "air_ground_control"       : 'sometimes|nullable|in:0,1,2',
}
```
### data example:
```json
{
  "last_name": "ShipXXX",
  "email": "dddddd_new_email@gmail.com"
}
```
# Response

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "id": 336,
    "client_id": 1,
    "order_number": "1688736219",
    "internal_order": "1-13",
    "order_date": "2023-09-09 11:11:11",
    "status": 1,
    "order_status_id": 1,
    "order_type_id": 1,
    "processing_type_id": 2,
    "parent_id": null,
    "first_name": "j",
    "last_name": null,
    "email": null,
    "company": null,
    "telephone": null,
    "address1": "111",
    "address2": null,
    "address3": null,
    "postal_code": "kkkk",
    "apt_num1": null,
    "apt_num2": null,
    "city": "kkkkkkk",
    "province_id": 121,
    "country_id": 38,
    "reference1": null,
    "reference2": null,
    "packing_slip_note": null,
    "pick_up": 0,
    "inside_delivery": 0,
    "lift_gate_required": 0,
    "ready": 0,
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
    "temperature_control": 0,
    "hazmat": 0,
    "appointment_required": 0,
    "order_handling": 0,
    "signature_required": 0,
    "ambient_control": 0,
    "air_ground_control": 0,
    "ship_onpty3": 0,
    "pty3_account": null,
    "handling_instruction": null,
    "dangerous_goods": 0,
    "language_id": 1,
    "warehouse_id": 12,
    "carrier_id": null,
    "service_id": null,
    "packing_slips": null,
    "note": null,
    "custom_reference_no": null,
    "tote_id": null,
    "transaction": null,
    "created_by": "Genming Zhao",
    "updated_by": "Genming Zhao",
    "created_at": "2023-07-07T13:23:39.000000Z",
    "updated_at": "2023-07-07T13:28:51.000000Z",
    "label_provided": 0,
    "shipping_label_file": null,
    "tracking_number": null,
    "created_by_name": null,
    "client_po": null,
    "carrier_service": null,
    "picking_method_id": 1,
    "client_order_id": null,
    "proxpert_import_at": null,
    "carrier": null,
    "trackings": null,
    "warehouse_name": "3DM - AVRO",
    "client_name": "Group 3-DM",
    "order_items": [
      {
        "id": 579,
        "order_id": 336,
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
        "created_at": "2023-07-16T19:23:20.000000Z",
        "sale_price": "3.00"
      }
    ]
  }
}
```

