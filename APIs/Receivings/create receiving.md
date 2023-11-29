# Create a new receiving record

`Method: POST`


`endpoint: api/v1/orders`

### data body

```json
{
  "client_id"                : "required|exists:clients,id",
  "order_number"             : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "order_date"               : "required|date_format:Y-m-d H:i:s",
  "first_name"               : "required|string|max:".Constant::MAX_STRING_LENGTH,
  "address1"                 : "required|string|max:".Constant::MAX_TEXT_LENGTH,
  "order_status_id"          : "sometimes|exists:order_statuses,id",
  "order_stage_id"           : "sometimes|exists:order_stages,id",
  "postal_code"              : "required|string|max:".Constant::MAX_STRING_LENGTH,
  "city"                     : "required|string|max:".Constant::MAX_STRING_LENGTH,
  "province_id"              : "required|exists:provinces,id",
  "country_id"               : "required|exists:countries,id",
  "telephone"                : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "last_name"                : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "company"                  : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "email"                    : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "reference1"               : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "reference2"               : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "packing_slip_note"        : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "items"                    : "required|array",
  "items.*"                  : "required|array",
  "items.*.quantity_ordered" : "required_with:items|integer|min:1",
  "items.*.uom_type_id"      : "required_with:items|exists:uom_types,id",//each, box, or pallet.
  "items.*.descriptions"     : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "items.*.lot"              : "sometimes|nullable|string|exists:receiving_items,lot|max:".Constant::MAX_STRING_LENGTH,
  "items.*.unit_value"       : "sometimes|nullable|numeric|min:0|max:".Constant::MAX_NUM,
  "items.*.sku"              : "nullable|exists:items,sku|max:".Constant::MAX_STRING_LENGTH,
  "items.*.item_id"          : "required_without:items.*.sku|exists:items,id|max:".Constant::MAX_STRING_LENGTH,
  "apt_num1"                 : "sometimes|string|nullable|max:".Constant::MAX_STRING_LENGTH,
  "apt_num2"                 : "sometimes|string|nullable|max:".Constant::MAX_STRING_LENGTH,
  "address2"                 : "sometimes|string|nullable|max:".Constant::MAX_STRING_LENGTH,
  "pick_up"                  : "sometimes|nullable|boolean",
  "inside_delivery"          : "sometimes|nullable|boolean",
  "lift_gate_required"       : "sometimes|nullable|boolean",
  "process_date"             : "sometimes|nullable|date",
  "handling_priority"        : "sometimes|nullable|boolean",
  "processing_priority"      : "sometimes|nullable|boolean",
  "temperature_control"      : "sometimes|nullable|in:0,1,2",
  "hazmat"                   : "sometimes|nullable|boolean",
  "appointment_required"     : "sometimes|nullable|boolean",
  "order_handling"           : "sometimes|nullable|boolean",
  "handling_instruction"     : "sometimes|nullable|string|max:".Constant::MAX_TEXT_LENGTH,
  "dangerous_goods"          : "sometimes|nullable|boolean",
  "language_id"              : "sometimes|nullable|exists:languages,id",
  "warehouse_id"             : "sometimes|nullable|exists:warehouses,id",
  "transaction"              : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "carrier_id"               : "sometimes|nullable|exists:carriers,id",
  "service_id"               : "sometimes|nullable|exists:services,id",
  "note"                     : "sometimes|nullable|string|max:".Constant::MAX_TEXT_LENGTH,
  "custom_reference_no"      : "sometimes|nullable|string|max:".Constant::MAX_STRING_LENGTH,
  "deliver_by_date"          : "sometimes|nullable|date_format:Y-m-d",
  "signature_required"       : 'sometimes|nullable|boolean',
  "ambient_control"          : 'sometimes|nullable|boolean',
  "air_ground_control"       : 'sometimes|nullable|in:0,1,2',
  "ship_onpty3"              : 'sometimes|nullable|boolean',
  "pty3_account"             : "sometimes|nullable|string|max:".Constant::MAX_TEXT_LENGTH,
  "client_po"                : "sometimes|nullable|string|max:".Constant::MAX_TEXT_LENGTH,
  "picking_method_id"        : "nullable|exists:picking_methods,id",
  "processing_type_id"       : "nullable|exists:processing_types,id",
}
```
### data example

```json
{
    "client_id": 1,
    "order_date": "2023-09-09 11:11:11",
    "first_name": "jon",
    "address1": "222 ave mntril",
    "postal_code": "kkkk",
    "city": "kkkkkkk",
    "province_id": 121,
    "country_id": 38,
    "order_items": [
         {
             "item_id": 1,
             "quantity_ordered": 1,
             "uom_type_id":1
         }
    ]
}
```
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